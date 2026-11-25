## UE Marketplace - Review Add

URL: https://www.unrealengine.com/marketplace/api/review/:offerId/:type/add <br/>
Method: POST <br/>
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

## Parameters

`title`: obvious <br/>
`content`: obvious <br/>
`targetOwner`: Account Id of creator

---

*Example Response*

```json
{
  "status": "OK",
  "data": true
}
```
