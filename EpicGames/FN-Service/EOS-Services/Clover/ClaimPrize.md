## FN EOS Clover Service: Claim Reserved Prize

URL: https://fngw-svc-ds-prod.ol.epicgames.com/clover/api/v1/ds/deployments/:deploymentId/domains/FN1/sessions/:sessionId/prizes/:prizeId/prize-reservation/claim \
Method: PUT \
Auth Required: Yes (No specific perm. Needs dedicated-server token)

```json
{
  "accountIds": ["a38e15a0fb474e45b8e95cd2093a7b62"]
}
```

## Path Parameters

`deploymentId`: The Deployment Id from env configuration, for `live-fn` it is `62a9473a2dca46b29ccf17577fcf42d7` <br/>
`sessionId`: Session where reward was obtained
`prizeId`: Unknown format but the id of the prize to be reserved (one of the delilah prizes)

---
