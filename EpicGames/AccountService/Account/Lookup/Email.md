## Account Service - Lookup by Email

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/email/:email \
Method: GET \
Auth Required: Yes (~~`account:public:account:byEmail`~~ `account:public:account:lookup:email READ`)

## Path Parameters

`email`: The Email to search for

---

_Example Response_

```json
{
  "id": "94b1569506b04f9f8557af611e8c5e47",
  "displayName": "lele stw moment",
  "externalAuths": {}
}
```

> Strict Ratelimit: 3 in 600 seconds

Has been deprecated as of 14.01.2023 (dd-MM-yyyy) due to data protection of e.g. underage children.
