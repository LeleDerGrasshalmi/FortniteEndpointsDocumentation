## Account Service - Public Key

URL: https://account-public-service-prod.ol.epicgames.com/account/api/publickeys/:thumbprint \
Method: GET \
Auth Required: No

## Path Parameters

`thumbprint`: The Public or Private Key Thumbprint, e.g. 'WMS7EnkIGpcH9DGZsv2WcY9xsuFnZCtxZjj4Ahb-\_8E' ('kid' from eg1 JWT Header)

---

_Example Response_

```json
{
  "kty": "RSA",
  "e": "AQAB",
  "kid": "WMS7EnkIGpcH9DGZsv2WcY9xsuFnZCtxZjj4Ahb-_8E",
  "n": "l6XI48ujknQQlsJgpGXg4l2i_DuUxuG2GXTzkOG7UtX4MqkVBCfW1t1JIIc8q0kCInC2oBwhC599ZCmd-cOi0kS7Aquv68fjERIRK9oCUnF_lJg296jV8xcalFY0FOWX--qX3xGKL33VjJBMIrIu7ETjj06s-v4li22CnHmu2lDkrp_FPTVzFscn-XRIojqIFb7pKRFPt27m12FNE_Rd9bqlVCkvMNuE7VTpTOrSfKk5B01M5IuXKXk0pTAWnelqaD9bHjAExe2I_183lp_uFhNN4hLTjOojxl-dK8Jy2OCPEAsg5rs9Lwttp3zZ--y0sM7UttN2dE0w3F2f352MNQ"
}
```
