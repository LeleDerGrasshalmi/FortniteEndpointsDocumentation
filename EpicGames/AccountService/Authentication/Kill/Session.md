## Account Service - Auth: Kill Session

URL: https://account-public-service-prod.ol.epicgames.com/account/api/oauth/sessions/kill/:session \
Method: DELETE \
Auth Required: Yes

## Parameters

`session`: string, the Access Token of the Session

## Query Parameters

`killAllWithSameSource`: bool, requires the `account:token:otherSessionsWithSameSourceForAccount DELETE` permission
