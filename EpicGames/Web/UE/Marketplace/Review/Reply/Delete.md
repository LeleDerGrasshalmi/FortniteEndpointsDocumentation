## UE Marketplace - Delete

URL: https://www.unrealengine.com/marketplace/api/review/:type/:replyId \
Method: DELETE \
Auth Required: Yes

## Path Parameters

`type`: the Type of the review (reviews,questions,replies)
`replyId`: the replyId of the review

## Query Parameters
`topicId`: the TopicId of the review

---

_Example Response_

```json
{
    "status": "OK",
    "data": true
}
```