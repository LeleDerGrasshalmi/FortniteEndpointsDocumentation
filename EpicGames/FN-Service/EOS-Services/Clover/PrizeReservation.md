## FN EOS Clover Service: Prize Reservation

URL: https://fngw-svc-ds-prod.ol.epicgames.com/clover/api/v1/ds/deployments/:deploymentId/domains/FN1/sessions/:sessionId/prizes/:prizeId/prize-reservation \
Method: PUT \
Auth Required: Yes (No specific perm. Needs dedicated-server token)

```json
{
  "quantity": 1,
  "expiresAt": ""
}
```

## Path Parameters

`deploymentId`: The Deployment Id from env configuration, for `live-fn` it is `62a9473a2dca46b29ccf17577fcf42d7` <br/>
`sessionId`: Session where reward was obtained
`prizeId`: Unknown format but the id of the prize to be reserved (one of the delilah prizes)

---
