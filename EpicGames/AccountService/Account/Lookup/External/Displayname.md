## Account Service - Lookup by External Display Name

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/lookup/externalAuth/:externalAuthType/displayName/:displayName \
Method: GET \
Auth Required: Yes (`account:public:account:lookup:externalDisplayName:{externalAuthType} READ`)

## Query Parameter

`caseInsensitive`: boolean (optional), just make it always true, theres no reason to care about the exact case

## Path Parameter

`externalAuthType`: See via [External Auth Readme](../../ExternalAuth/README.md) <br/>
`displayName`: External Provider User Displayname
