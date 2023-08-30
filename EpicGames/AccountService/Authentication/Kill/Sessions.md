## Account Service - Auth: Kill Sessions

URL: https://account-public-service-prod.ol.epicgames.com/account/api/oauth/sessions/kill \
Method: DELETE \
Auth Required: Yes

### Query Parameters

`killType`: See below

| Type                          | Permission                                                                                                          | Description                                                                                                |
| ----------------------------- | ------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| OTHERS_ACCOUNT_CLIENT_SERVICE | `Account`: account:token:otherSessionsForAccountClientService DELETE                                                | Kills all other Auth Sessions for the same Client for Service for the logged in Account (used in Fortnite) |
| OTHERS_ACCOUNT_CLIENT         | `Account`: account:token:otherSessionsForAccountClient DELETE                                                       | Kills all other Auth Sessions for the same Client for the logged in Account                                |
| OTHERS_SAME_SOURCE_ID         | `Account`: account:token:otherSessionsWithSameSourceId DELETE                                                       | Kills all session from the same source???                                                                  |
| OTHERS                        | `Client`: account:token:otherSessionsForClient DELETE <br/> `Account`: account:token:otherSessionsForAccount DELETE | Kills all Other Auth Sessions                                                                              |
| ALL                           | `Client`: account:token:allSessionsForClient DELETE <br/> `Account`: account:token:allSessionsForAccount DELETE     | Kills every Auth Session (including current Session)                                                       |
| ALL_ACCOUNT_CLIENT            | `Account`: account:token:allSessionsForAccountClient DELETE                                                         | Kills every Auth Session for this Client for the logged in Account (including the current Session)         |

---

_Example Response_: Status 204
