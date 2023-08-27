## UE Marketplace - Review Delete

URL: https://www.unrealengine.com/marketplace/api/review/:offerId/reviews/:topicId \
Method: DELETE \
Auth Required: Yes

### Query Parameters

`type`: the Type of the review (reviews,questions,replies)

## Path Parameters

`offerId`: the Id of the Offer
`topicId`: the TopicId of the review

---

_Example Response_

```json
{
    "status": "OK",
    "data": true
}
```