## FN EOS Locker Service: Change Companion Name

URL: https://fngw-svc-gc-livefn.ol.epicgames.com/api/locker/v4/:deploymentId/account/:accountId/companion-name \
Method: PATCH \
Auth Required: Yes (`locker:{accountId} UPDATE`)

```json
{
  "cosmeticItemId": "templateId:GUID",
  "companionName": "New Companion Name"
}
```

## Path Parameters

`deploymentId`: The Deployment Id from env configuration, for `live-fn` it is `62a9473a2dca46b29ccf17577fcf42d7` <br/>
`accountId`: Your Account Id

---

_Example Response_

`Status 204`
