## Friends Service - Mutual Friends

URL: https://friends-public-service-prod.ol.epicgames.com/friends/api/v1/:accountId/friends/:friendId/mutual \
Method: GET \
Auth Required: Yes (`friends:{accountId} READ`)

## Path Parameters

`accountId`: Your Account Id <br/>
`friendId`: Friend Account Id

---

_Example Response_

```json
["736120836fd04049b9d9fca94d35898e", "6c10bed53c144a17adc797ec43083cf8"]
```

> Returns Mutual friends account Ids
