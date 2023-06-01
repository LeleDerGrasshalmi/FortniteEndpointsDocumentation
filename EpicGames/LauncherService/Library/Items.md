## Launcher Service - Library: Items (Proxy)

URL: https://launcher-public-service-prod06.ol.epicgames.com/launcher/api/public/library/items \
Method: GET \
Auth Required: Yes (`launcher:library:items READ`)

## Query Parameters

`excludeNs`: optional, namespaces to exclude, can be used multiple times <br/>
`limit`: optional, how many records to include <br/>
`platform`: optional, only include items that are available on the specified platform, e.g. `Windows` or `Android` <br/>
`nextCursor`: optional, from the metadata to see more records

---

_Example Response_

```json
{
  "records": [
    {
      "namespace": "08ae29e4f70a4b62aa055e383381aa82",
      "catalogItemId": "1addbe9a36af44b2868133287a3673c0",
      "appName": "0a20ccd3f1b3464da750a4dbf8c80d7c"
    }
  ],
  "responseMetadata": {
    "nextCursor": "eyJlbnRpdGxlbWVudElkIjoiZTVlYzBhZjcyZjMxNDUzYmE3Y2VhNDVkZTY5NjliZWIiLCJwbGF0Zm9ybUZpbHRlciI6bnVsbCwiZXhjbHVkZU5hbWVzcGFjZXMiOlsid2V4IiwibGF2ZW5kZXIiLCJsZWxlLWRvY3MiXX0="
  }
}
```
