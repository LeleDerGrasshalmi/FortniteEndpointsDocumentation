## UE Marketplace - Review Edit

URL: https://www.unrealengine.com/marketplace/api/review/:offerId/:type/edit \
Method: POST \
Auth Required: Yes

```json
{
  "title": "title m",
  "content": "description m",
  "targetOwner": "accountid",
  "type": "type",
  "topicId": "topic"
}
```

## Path Parameters

`offerId`: The Id of the Offer <br/>
`type`: The Type of the review (reviews,questions,replies)

## Parameters

`title`: obvious <br/>
`content`: obvious <br/>
`targetOwner`: account id of creator <br/>
`type`: The Type of the review (reviews,questions,replies) <br/>
`topicId`: The TopicId of the review

---

_Example Response_

```json
{
  "status": "OK",
  "data": true
}
```
