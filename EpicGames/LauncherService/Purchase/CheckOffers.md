## Launcher Service - Purchase: Check Offers

URL: https://launcher-public-service-prod06.ol.epicgames.com/launcher/api/public/purchase/offers/bulk \
Method: POST \
Auth Required: Yes (~~`purchase:offers READ`~~ `launcher:purchase:offers READ`)

## Headers

`Content-Type`: `application/x-www-form-urlencoded`

<br/>

```
nsOfferId=aa:bb&nsOfferId=cc:dd
```

## Parameters

`nsOfferId`: Can be used multiple times, format: `{namespace}:{offerId}`

---

_Example Response_

```json
{
  "fn:554f1353544248d8af51cc42df4f0a42": {
    "nsOfferIds": ["fn:554f1353544248d8af51cc42df4f0a42"],
    "missingPrerequisiteItems": [],
    "satisfiesPrerequisites": true
  }
}
```

> This endpoint is now deprecated
