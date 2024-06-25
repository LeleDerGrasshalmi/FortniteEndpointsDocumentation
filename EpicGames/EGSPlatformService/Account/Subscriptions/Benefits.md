## EGS Platform Service - Subscription Benefits

URL: https://egs-platform-service.store.epicgames.com/api/v1/private/egs/products/:productId/offers/:offerId/subscriptions/benefits \
Method: GET \
Auth Required: Yes (apparently `subscription:public:subscription-def READ`)

## Query Parameters

`store`: (required) valid Catalog Service Stores, e.g. `EGS`

## Path Parameters

`productId`: Self explaining, e.g. `prod-fn` for fortnite <br/>
`offerId`: The offer id from catalog service of the `SUBSCRIPTION` offer <br/>

---

_Example Response (success)_

```json
{
  "applicableBenefits": [],
  "offerId": "9ec21a8d4f744f8b938fbf79d02d40b9",
  "sandboxId": "fn"
}
```
