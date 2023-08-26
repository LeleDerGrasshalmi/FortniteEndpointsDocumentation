## UE Web - Edit

URL: https://www.unrealengine.com/marketplace/api/review/:offerId/:type/edit \
Method: POST \
Auth Required: Yes

## Path Parameters

`offerId`: the Id of the Offer
`type`: the Type of the review (reviews,questions,replies)

## Body Parameters
`type`: the Type of the review (reviews,questions,replies)
`topicId`: the TopicId of the review

```json
{
    "title": "title m",
    "content": "description m",
    "targetOwner": "account id of creator",
    "type":"type",
    "topicId":"topic"
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