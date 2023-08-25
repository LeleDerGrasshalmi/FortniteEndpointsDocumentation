## Library Service - State Token

URL: https://library-service.live.use1a.on.epicgames.com/library/api/public/stateToken/:stateToken/status \
Method: GET \
Auth Required: Yes (`library:public:stateToken:status READ`)

## Path Parameters

`stateToken`: The State Token returned by another Library Service API (e.g. [Library Items](./LibraryItems.md)), this is a UUIDv4

---

_Example Response (Valid)_

```json
{
  "valid": true
}
```

_Example Response (Not Valid)_

```json
{
  "valid": false
}
```
