## Account Service - Auth: Kill Session

URL: https://account-public-service-prod.ol.epicgames.com/account/api/oauth/sessions/kill/:session <br/>
Method: DELETE <br/>
Auth Required: Yes

## Path Parameters

`session`: The Access Token of the Session

## Query Parameters

`killAllWithSameSource`: bool, requires the `account:token:otherSessionsWithSameSourceForAccount DELETE` Permission

---

*Example Response*: Status 204
