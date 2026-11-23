## Wex Service - Cloudstorage: System File Content

URL: https://wex-public-service-live-prod.ol.epicgames.com/wex/api/cloudstorage/system/:uniqueFilename <br/>
Method: GET <br/>
Auth Required: Yes (`wexp:cloudstorage:system:{uniqueFilename} READ`)

## Path Parameters

`uniqueFilename`: The `uniqueFilename` from the List

---

*Example Response (DefaultEngine.ini)*

```ini
[OnlineSubsystemMcp.OnlineIdentityMcp]
bAllowMultiLogin=true
ExchangeRedirectUrl="/id/exchange?exchangeCode=`code&redirectUrl=`desturl"
```
