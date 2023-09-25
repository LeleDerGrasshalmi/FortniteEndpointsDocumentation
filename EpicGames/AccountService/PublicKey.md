## Account Service - Public Key

URL: https://account-public-service-prod.ol.epicgames.com/account/api/publickeys/:thumbprint \
Method: GET \
Auth Required: No

## Path Parameters

`thumbprint`: The Public or Private Key Thumbprint, e.g. `g__VKjSSmqJ0xZj1RYkLGKQ7dnHiM9MLhFVwKPySDB4` (`kid` from eg1 JWT Header) or `WMS7EnkIGpcH9DGZsv2WcY9xsuFnZCtxZjj4Ahb-_8E` (`kid` from epic_id JWT Header)

---

_Example Response_

```json
{
  "kty": "RSA",
  "e": "AQAB",
  "kid": "g__VKjSSmqJ0xZj1RYkLGKQ7dnHiM9MLhFVwKPySDB4",
  "n": "2QqXCndTrbOC8YqRcZPhixXFrGgL5cUOWP7IJgroYIgQ4JWIrXIY89zs0QvmdDdwHvp_CKRnfin6nsNhYKzVCghDuZ5Es5Zn7YbIzU6TGhYmQ0xE84AIgTh5Z-1j4K1aFxGLGajftbIfltwKHXLEwGd9Amylb0_Nd_KlQvmYR_3Cu85MKiQCzpvyP0Ex07WCL9rDeo4rct6jztrE31PrrM7KXBY9dV_OrQWsq72thsGrCYMx-vcMwXFZu-wtWzCJH1LwWuMW6yOcu-ipndYpLTKtr0S57izs6sSYS3nj2xJGWp_rLK7Xrqb6X8raFuExMG3kgb17scLqv5v51cvYZ3Aqw9Q0RGkeTejoku7G970EDxC-abrgVfIHePBklFcFviyNBKE0IxWZjt1MQENRh9lJOPXP_0WAnm3NvSDSVqSzBYxggPA_dtUUo6IZ-m-cX3NVyeBEkkfZXRgWhXfW7F9GZ9SvpvXdjweBCUO9m0mwPzFXJwt1FGtJYnkSd5M00D3srX2FdulPfnOZhXSSSmKSEgpetq0UGu4JiVAZmPELo9k5jrzA_9kuyRC_AnIIcKSZH1sTVacIxW0fsufxJbpnqWs3jGGPQXlBHteAr8PZ3PQ0REjorXgdMICuv_dSN_HrGATthnqEaOnF3Nk5aNBhVAFHpe-j7q8nCjw8gbc"
}
```
