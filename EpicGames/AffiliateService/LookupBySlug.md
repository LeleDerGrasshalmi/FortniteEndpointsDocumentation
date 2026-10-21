## Affiliate Service - Affiliates: Lookup by Slug

Look up a Support-A-Creator code (slug). Useful to validate a code before applying it with the [`SetAffiliateName`](../FN-Service/Game/Profile/Operations/SetAffiliateName.md) MCP operation. Lookups are case-insensitive.

URL: https://affiliate-public-service-prod.ol.epicgames.com/affiliate/api/public/affiliates/slug/:slug \
Method: GET \
Auth Required: Yes (any token, `client_credentials` works)

## Path Parameters

`slug`: The Support-A-Creator code

---

_Example Response_

```json
{
  "id": "4735ce9132924caf8a5b17789b40f79c",
  "slug": "ninja",
  "displayName": "Ninja",
  "status": "ACTIVE",
  "verified": false
}
```

_Example Response (code not found, `404`)_

```json
{
  "errorCode": "errors.com.epicgames.ecommerce.affiliate.not_found",
  "errorMessage": "Sorry, the affiliate cannot be found by slug [thiscodedoesnotexist123].",
  "messageVars": [],
  "numericErrorCode": 47010,
  "originatingService": "com.epicgames.ecp",
  "intent": "prod"
}
```
