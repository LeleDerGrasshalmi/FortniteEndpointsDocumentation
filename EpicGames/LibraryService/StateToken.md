## Library Service - State Token

URL: https://library-service.live.use1a.on.epicgames.com/library/api/public/stateToken/:stateToken/status <br/>
Method: GET <br/>
Auth Required: Yes (`library:public:stateToken:status READ`)

## Path Parameters

`stateToken`: The State Token returned by another Library Service API (e.g. [Library Items](./LibraryItems.md)), this is a UUIDv4

---

*Example Response (Valid)*

```json
{
  "valid": true
}
```

*Example Response (Not Valid)*

```json
{
  "valid": false
}
```
