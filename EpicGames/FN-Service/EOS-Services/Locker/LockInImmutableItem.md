## FN EOS Locker Service: Lock In Immutable Item

URL: https://fngw-svc-gc-livefn.ol.epicgames.com/api/locker/v4/:deploymentId/account/:accountId/lock-in-immutable-item/:itemIdentifier \
Method: POST \
Auth Required: Yes (`locker:{accountId} UPDATE`)

```json
{
  "variants": {
    "Immutable.RichColor": {
      "variantTag": "RichColor",
      "additionalData": "3D3215FD3D3215FD3D3215FD3F800000"
    },
    "Immutable.RichColor2": {
      "variantTag": "RichColor",
      "additionalData": "3F5B37223F5A61073F6666663F800000"
    },
    "Immutable.RichColor3": {
      "variantTag": "RichColor",
      "additionalData": "3E3216403D5CC5333CDCD4ED3F800000"
    },
    "Immutable.AdditivePose": {
      "variantTag": "Stage0"
    }
  }
}
```

## Path Parameters

`deploymentId`: The Deployment Id from env configuration, for `live-fn` it is `62a9473a2dca46b29ccf17577fcf42d7` <br/>
`accountId`: Your Account Id <br/>
`itemIdentifier`: Composite item identifier containing `{templateId}:{itemGUID}` from profile. Example value: `CosmeticMimosa:companion_sitplant:e28d2412-7f77-4e99-926f-18976abd8a70`

---

_Example Response_

`Status 204`
