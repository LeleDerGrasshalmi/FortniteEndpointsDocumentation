## UE Marketplace - Edit Review Reply

URL: https://www.unrealengine.com/marketplace/api/review/:type/:replyId \
Method: PUT \
Auth Required: Yes

## Path Parameters

`type`: the Type of the review (reviews,questions,replies) <br/>
`replyId`: the replyId of the review

```json
{
    "title": "title m",
    "content": "description m",
    "topicId": "topic id"
}
```

## Parameters

`title`: obvious <br/>
`content`: obvious <br/>
`topicId`: the TopicId of the review

---

_Example Response_

```json
{
    "status": "OK",
    "data": true
}
```
