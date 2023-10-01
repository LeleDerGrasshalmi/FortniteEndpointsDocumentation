## UE Marketplace - Review Add

URL: https://www.unrealengine.com/marketplace/api/review/:offerId/:type/add \
Method: POST \
Auth Required: Yes

```json
{
  "title": "title m",
  "content": "description m",
  "targetOwner": "account id of creator"
}
```

## Path Parameters

`offerId`: The Id of the Offer <br/>
`type`: The Type of the review (reviews,questions,replies)

## Path Parameters

`title`: obvious <br/>
`content`: obvious <br/>
`targetOwner`: Account Id of creator

---

_Example Response_

```json
{
  "status": "OK",
  "data": true
}
```
