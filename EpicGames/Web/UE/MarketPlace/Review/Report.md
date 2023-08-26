## UE Web - Report Send

URL: https://www.unrealengine.com/marketplace/api/review/:type/:topicId/report \
Method: POST \
Auth Required: Yes

## Path Parameters

`type`: the Type of the review (reviews,questions,replies)
`topicId`: the TopicId of the review

## Body Parameters

`abuseType`: the type (Unwanted spam,Sexually Explicit material,Hate speech / graphic violence,Harassment,Inaccuracy)

```json
{
    "abuseType": "type",
    "content": "test"
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

## UE Web - Report Get

URL: https://www.unrealengine.com/marketplace/api/review/:type/:topicId/report \
Method: GET \
Auth Required: Yes

## Path Parameters

`type`: the Type of the review (reviews,questions,replies)
`topicId`: the TopicId of the review

---

_Example Response_

```json
{
    "status": "OK",
    "data": ""
}
```