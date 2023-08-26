## UE Web - Vote

URL: https://www.unrealengine.com/marketplace/api/review/:type/:topicId/vote \
Method: POST \
Auth Required: Yes

## Path Parameters

`type`: the Type of the review (reviews,questions,replies)
`topicId`: the TopicId of the review

```json
{
    "isHelpful": true
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