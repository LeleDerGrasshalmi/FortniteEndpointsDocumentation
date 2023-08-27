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

`offerId`: the Id of the Offer
`type`: the Type of the review (reviews,questions,replies)

---

_Example Response_

```json
{
    "status": "OK",
    "data": true
}
```