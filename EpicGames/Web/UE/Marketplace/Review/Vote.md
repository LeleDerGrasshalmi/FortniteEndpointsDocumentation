## UE Marketplace - Review Vote

URL: https://www.unrealengine.com/marketplace/api/review/:type/:topicId/vote <br/>
Method: POST <br/>
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

*Example Response*

```json
{
  "status": "OK",
  "data": true
}
```
