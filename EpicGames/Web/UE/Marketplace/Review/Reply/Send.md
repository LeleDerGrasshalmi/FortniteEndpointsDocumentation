## UE Marketplace - Send Review Reply

URL: https://www.unrealengine.com/marketplace/api/review/:type/:topicId/reply \
Method: POST \
Auth Required: Yes

```json
{
    "content": "description m"
}
```

## Path Parameters

`type`: the Type of the review (reviews,questions,replies) <br/>
`topicId`: the TopicId of the review

## Parameters

`content`: obvious

---

_Example Response_

```json
{
    "status": "OK",
    "data": true
}
```
