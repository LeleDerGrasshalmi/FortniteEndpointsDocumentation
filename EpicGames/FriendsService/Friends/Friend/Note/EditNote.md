## Friends Service - Set Note

URL: https://friends-public-service-prod.ol.epicgames.com/friends/api/v1/:accountId/friends/:friendId/note \
Method: PUT \
Auth Required: Yes (`friends:{accountId} UPDATE`)

## Headers

`Content-Type`: text/plain

---

_The body is the new note text (min 3, max 255 characters)_

```
hello from lele's epic api docs
```

## Path Parameters

`accountId`: Your Account Id <br/>
`friendId`: Friend Account Id

---

_Example Response_: Status 204
