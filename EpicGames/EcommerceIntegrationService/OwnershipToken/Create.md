## Ecommerce Integration Service - Ownership Token

Creates an ownership verification token for catalog items. Games whose catalog item has the custom attribute `OwnershipToken` set to `true` (e.g. Hogwarts Legacy, Just Cause 4) expect it at launch, written to a file passed with `-epicovt=<path>`.

URL: https://ecommerceintegration-public-service-ecomprod02.ol.epicgames.com/ecommerceintegration/api/public/platforms/EPIC/identities/:accountId/ownershipToken \
Method: POST \
Auth Required: Yes (Bearer access token)

## Headers

`Content-Type`: application/x-www-form-urlencoded

## Path Parameters

`accountId`: Your Account Id

## Body

`nsCatalogItemId`: `{namespace}:{catalogItemId}` of the item

---

_Example Response_

```json
{
  "token": "egoc1~eyJraWQiOiJWbWdpMDFoQ2V2dXVEbUtWZFZubXphWnhpT2lBa0dEZWdRQmdDdWc4dkRZIiwiYWxnIjoiUlM1MTIifQ.eyJzdWIiOi..."
}
```

The token is `egoc1~` followed by a JWT (RS512) valid for 5 minutes. Decoded payload:

```json
{
  "sub": "94b1569506b04f9f8557af611e8c5e47",
  "ip": "0.0.0.0",
  "clid": "34a02cf8f4414e29b15921876da36f9a",
  "ent": [
    {
      "namespace": "e97659b501af4e3981d5430dad170911",
      "catalogItemId": "864c7bc2c2394f7dbd1b534aa068ff56",
      "owned": true
    }
  ],
  "exp": 1792033555,
  "iat": 1792033255,
  "jti": "a54701aa3ffd4477b9e6e085b86a72d3"
}
```

An item that is not owned still returns 200, with `"owned": false`. A request without `nsCatalogItemId` returns 500 `errors.com.epicgames.common.server_error`.
