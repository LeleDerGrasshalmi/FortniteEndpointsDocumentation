## EGS Platform Service - Subscription Benefits

URL: https://egs-platform-service.store.epicgames.com/api/v1/private/egs/products/:productId/offers/:offerId/subscriptions/benefits <br/>
Method: GET <br/>
Auth Required: Yes (apparently `subscription:public:subscription-def READ`)

## Path Parameters

`productId`: Self explaining, e.g. `prod-fn` for fortnite <br/>
`offerId`: The offer id from catalog service of the `SUBSCRIPTION` offer <br/>

## Query Parameters

`store`: (required) valid Catalog Service Stores, e.g. `EGS`

---

*Example Response (success)*

```json
{
  "applicableBenefits": [],
  "offerId": "9ec21a8d4f744f8b938fbf79d02d40b9",
  "sandboxId": "fn"
}
```
