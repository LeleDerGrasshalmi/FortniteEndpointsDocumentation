## UE Web - Edit

URL: https://www.unrealengine.com/marketplace/api/review/:type/:replyId \
Method: PUT \
Auth Required: Yes

## Path Parameters

`type`: the Type of the review (reviews,questions,replies)
`replyId`: the replyId of the review

```json
{
    "title": "title m",
    "content": "description m",
    "topicId": "topic id"
}
```

---

_Example Response_

```json
{
    "status": "OK",
    "data": true
}
```
