## Account Web - Vbucks Card History

URL: https://www.epicgames.com/account/v2/payment/vbucks-card-code-redemption-history?locale=en-US&page=0 \
Method: GET \
Auth Required: Yes

---

_Example Response_

```json
{
    "success": true,
    "elements": [
        {
            "pin": "2AZ36JR8XJST647S",
            "productInfo": { "namespace": "fn", "offerId": "9164ff9b44f74034b94b01203bee2d11" },
            "platform": "PSN",
            "date": "2021-07-24T01:27:17.797Z",
            "description": "[Card] 1,000 V-Bucks",
            "secondaryCode": "GJBD-JANB-FRAT"
        }
    ],
    "paging": { "count": 10, "start": 0, "total": 8 },
    "isPaginated": false
}
```
