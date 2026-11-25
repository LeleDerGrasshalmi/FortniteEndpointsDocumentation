## UE Marketplace - Send Review Reply

URL: https://www.unrealengine.com/marketplace/api/review/:type/:topicId/reply <br/>
Method: POST <br/>
Auth Required: Yes

```json
{
  "content": "description m"
}
```

## Path Parameters

`type`: The Type of the Review (reviews, questions, replies) <br/>
`topicId`: The Topic Id of the Review

## Parameters

`content`: obvious

---

*Example Response*

```json
{
  "status": "OK",
  "data": true
}
```
