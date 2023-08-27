## UE Web - Send

URL: https://www.unrealengine.com/marketplace/api/review/:type/:topicId/reply \
Method: POST \
Auth Required: Yes

```json
{
    "content": "description m"
}
```

## Path Parameters

`type`: the Type of the review (reviews,questions,replies)
`topicId`: the TopicId of the review

---

_Example Response_

```json
{
    "status": "OK",
    "data": true
}
```