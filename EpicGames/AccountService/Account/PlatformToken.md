## Account Service - Get Platform Token

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/:accountId/platformToken/:externalAuthType/:clientId \
Method: POST \
Auth Required: Yes (`account:public:account READ`)

```json
{
  "exchangeCode": ""
}
```

## Path Parameters

`accountId`: Your Account Id <br/>
`externalAuthType`: See [External Auth Types](../Authentication/GrantTypes/external_auth.md#body) <br/>
`clientId`: Unknown Value <br/>

## Parameters

`exchangeCode`: Issued by the External Provider, see the [External Auth Types](../Authentication/GrantTypes/external_auth.md#body) for more Info

---

_Example Response_

```json
{
  "accessToken": "ep1~eyJraWQiOiJ0RkMyVUloRnBUTV9FYTNxY09kX01xUVQxY0JCbTlrRkxTRGZlSmhzUkc4IiwiYWxnIjoiUFMyNTYifQ.eyJ0IjoicCIsInBsYXQiOiJwc24iLCJlbmMiOiJlcDF-ZXlKcmFXUWlPaUpGUmtoUlpUUkdNMlpoY2xOaFRHWlVSalF5V2pKT2VUWjBjMlJsUW1WMVgwZzNhV0pMVW1GblUycGpJaXdpWlc1aklqb2lRVEV5T0VkRFRTSXNJbUZzWnlJNklsSlRRUzFQUVVWUUxUSTFOaUo5LkFrWkc4WXlYUVdmd1A0T3ZaT2FwYnJra2VuWGx4QnlzdXpuTE5hTnhSTk04NGtVdlZqUWtRSVEzRDZjVjEwZWFVZDFSS2s2bExzNjBqMXBhSUlxY2JJbjJsYkdkVVM1UlJkdEJtNktml2VklKY3b2k0UEV6WmRsVFk4dnA1VnZBRDEyRkdZRXMuTXNwUjJUWUJRVjd6V05zZXE3SUd1ZyIsImV4cCI6MTY4NjQyMzA2MH0.AGB5UUgDND8ykGjE42JVhgWmXU_OOgj8FbjFZvAaeF7qpzTlJt92A0unyE35mr7WgP18ZlNWl3H7fxgXPmk13jad",
  "expiresIn": 3598,
  "expiresAt": "2023-06-10T18:51:00.283Z"
}
```
