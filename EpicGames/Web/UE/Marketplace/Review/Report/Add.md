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

`type`: the Type of the review (reviews,questions,replies) <br/>
`topicId`: the TopicId of the review

## Parameters

`abuseType`: the type (Unwanted spam,Sexually Explicit material,Hate speech / graphic violence,Harassment,Inaccuracy)
`content`: writen reason

---

_Example Response_

```json
{
    "status": "OK",
    "data": true
}
```
