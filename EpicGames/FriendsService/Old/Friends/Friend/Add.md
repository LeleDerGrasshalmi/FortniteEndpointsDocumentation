## Friends Service - Accept Incoming / Send Outgoing

URL: https://friends-public-service-prod.ol.epicgames.com/friends/api/public/friends/:accountId/:friendId <br/>
Method: POST <br/>
Auth Required: Yes (`friends:{accountId} UPDATE`)

```json
{
  "pin": "123456"
}
```

## Path Parameters

`accountId`: Your Account Id <br/>
`friendId`: Friend Account Id

## Parameters

`pin`: The required parental controls pin, that is required when its configured, that friend management needs the pin

---

*Example Response (success)*: Status 204
