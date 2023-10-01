## UE Marketplace - Edit Review Reply

URL: https://www.unrealengine.com/marketplace/api/review/:type/:replyId \
Method: PUT \
Auth Required: Yes

```json
{
  "title": "title m",
  "content": "description m",
  "topicId": "topic id"
}
```

## Path Parameters

`type`: the Type of the review (reviews, questions, replies) <br/>
`replyId`: The Replay Id of the Review

## Parameters

`title`: obvious <br/>
`content`: obvious <br/>
`topicId`: The Topic Id of the Review

---

_Example Response_

```json
{
  "status": "OK",
  "data": true
}
```
