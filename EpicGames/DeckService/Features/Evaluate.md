## Deck - Evaluate Features

URL: https://distro-gateway-prod.ol.epicgames.com/deck/v1/features \
Method: POST \
Auth Required: No

## Body

```json
{
  "flags": {
    "presence-mode": "social-overlay",
    "quiet-hours-enabled": true,
    "self-update-mode": "disabled"
  },
  "context": {
    "kind": "multi",
    "machine": {
      "environment": "prod",
      "os": "windows",
      "arch": "x86_64",
      "currentVersion": "0.115.0+gd6d2ef8",
      "releaseChannel": "stable"
    },
    "user": {
      "anonymous": true
    }
  }
}
```

`flags`: Required. Object of flag key to default value <br/>
`context`: Machine attributes and an anonymous user

---

_Example Response_

```json
{
  "presence-mode": "social-overlay",
  "quiet-hours-enabled": false,
  "self-update-mode": "forced"
}
```

One entry per requested key. Unknown keys come back with the default that was sent.

_Example Response (no `flags`)_: Status 400

```json
{
  "message": "flags is a required parameter.",
  "correlationId": "e8391a70-0c8e-41ba-9e80-5519ea943512"
}
```
