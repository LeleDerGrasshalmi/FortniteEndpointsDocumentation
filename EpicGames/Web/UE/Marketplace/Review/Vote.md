## UE Marketplace - Review Vote

URL: https://www.unrealengine.com/marketplace/api/review/:type/:topicId/vote \
Method: POST \
Auth Required: Yes

```json
{
  "isHelpful": true
}
```

## Path Parameters

`type`: The Type of the review (reviews,questions,replies) <br/>
`topicId`: The TopicId of the review

## Parameters

`isHelpful`: vote boolean

---

_Example Response_

```json
{
  "status": "OK",
  "data": true
}
```
