## UE Marketplace - Send Review Report

URL: https://www.unrealengine.com/marketplace/api/review/:type/:topicId/report \
Method: POST \
Auth Required: Yes

```json
{
  "abuseType": "type",
  "content": "test"
}
```

## Path Parameters

`type`: The Type of the Review (reviews, questions, replies) <br/>
`topicId`: The Topic Id of the Review

## Parameters

`abuseType`: The type (Unwanted spam,Sexually Explicit material,Hate speech / graphic violence,Harassment,Inaccuracy)
`content`: The Reason

---

_Example Response_

```json
{
  "status": "OK",
  "data": true
}
```
