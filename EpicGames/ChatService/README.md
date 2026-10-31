# Chat Service

Text chat on the EOS API Gateway (`/epic/chat`). Conversation `type` values: `dm`, `group`, `epic_party` (party chats use `ep-{partyId}` as conversation id).

## Hosts

- api.epicgames.dev

## Message Signing

Messages are signed with an Ed25519 key that was registered at the [Public Key Service](../PublicKeyService/PublicKey/Register.md).

```json
{
  "message": {
    "body": "<base64 payload>"
  },
  "metadata": {
    "Sig": "<base64 ed25519 signature>",
    "Pub": "<jwt>",
    "TmV": "2"
  }
}
```

`message.body`: Standard base64 of the compact JSON payload below <br/>
`metadata.Sig`: Standard base64 of the Ed25519 signature over `message.body` + `\0` (UTF-8 bytes) <br/>
`metadata.Pub`: The `jwt` returned by [Register Public Key](../PublicKeyService/PublicKey/Register.md) <br/>
`metadata.TmV`: `2`

Payload (keys in this order, no whitespace):

```json
{"mid":"1e5d3c2b-6f70-4b8c-9dae-1f2a3b4c5d6e","sid":"c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60","rid":"GBD2ExampleConversationId00001","msg":"hello","tst":1792001306956,"seq":1,"rec":false,"mts":[],"cty":"Persistent"}
```

`mid`: Random UUID v4, same as the `sourceMsgId` query parameter <br/>
`sid`: Sender AccountId <br/>
`rid`: Conversation Id, omitted for the first direct message <br/>
`msg`: The message text <br/>
`tst`: Timestamp in milliseconds <br/>
`seq`: Sequence number, e.g. `1` <br/>
`rec`: `false` <br/>
`mts`: `[]` <br/>
`cty`: `Persistent`
