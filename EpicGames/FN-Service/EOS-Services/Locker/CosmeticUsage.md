## FN EOS Locker Service: Cosmetic Usage

URL: https://fngw-svc-gc-livefn.ol.epicgames.com/api/locker/v4/:deploymentId/account/:accountId/cosmetic-usage \
Method: GET \
Auth Required: Yes (`locker:items`)

## Path Parameters

`deploymentId`: The Deployment Id from env configuration, for `live-fn` it is `62a9473a2dca46b29ccf17577fcf42d7` <br/>
`accountId`: Your Account Id

---

_Example Response (shortened)_

```json
{
  "cosmeticUsage": {
    "AthenaBackpack:bid_610_elastichologram": {
      "lastUsedTimestamp": "2026-10-18T20:20:28.347558765Z",
      "usageCounter": 32
    },
    "AthenaCharacter:cid_619_athena_commando_f_techllama": {
      "lastUsedTimestamp": "2026-10-18T21:43:20.243411106Z",
      "usageCounter": 20
    },
    "AthenaDance:emoji_s34_lanternfest25": {
      "lastUsedTimestamp": "2026-10-18T20:20:28.347558765Z",
      "usageCounter": 32
    },
    "AthenaPickaxe:pickaxe_misttycoonhike": {
      "lastUsedTimestamp": "2026-10-18T21:43:20.243411106Z",
      "usageCounter": 20
    },
    "AthenaSkyDiveContrail:defaultcontrail": {
      "lastUsedTimestamp": "2026-10-18T21:43:20.243411106Z",
      "usageCounter": 51
    },
    "CosmeticMimosa:companion_sitplant:e3cdcd15-3aa7-42d7-a513-e3066b0c77ba": {
      "lastUsedTimestamp": "2026-10-18T21:43:20.243411106Z",
      "usageCounter": 51
    },
    "CosmeticMimosaC:companion_reactfx_sitplant": {
      "lastUsedTimestamp": "2026-10-17T02:19:18.701558070Z",
      "usageCounter": 2
    },
    "CosmeticShoes:shoes_yukongladtube": {
      "lastUsedTimestamp": "2026-10-18T21:43:20.243411106Z",
      "usageCounter": 22
    },
    "HomebaseBannerColor:defaultcolor22": {
      "lastUsedTimestamp": "2026-10-18T21:43:20.243411106Z",
      "usageCounter": 53
    },
    "HomebaseBannerIcon:endurancewave30theater04": {
      "lastUsedTimestamp": "2026-10-18T21:43:20.243411106Z",
      "usageCounter": 53
    },
    "SparksAura:sparksaura_centerstage": {
      "lastUsedTimestamp": "2026-10-18T20:20:28.347558765Z",
      "usageCounter": 31
    },
    "SparksBass:sparks_gatorceladon_bass": {
      "lastUsedTimestamp": "2026-10-18T21:43:20.243411106Z",
      "usageCounter": 53
    },
    "SparksDrums:sparks_drum_jadetowel": {
      "lastUsedTimestamp": "2026-10-18T21:43:20.243411106Z",
      "usageCounter": 53
    },
    "SparksGuitar:sparks_dryerase_guitar": {
      "lastUsedTimestamp": "2026-10-18T21:43:20.243411106Z",
      "usageCounter": 53
    },
    "SparksKeyboard:sparks_keytar_jadetowel": {
      "lastUsedTimestamp": "2026-10-18T21:43:20.243411106Z",
      "usageCounter": 53
    },
    "SparksMicrophone:sparks_mic_jadetowel": {
      "lastUsedTimestamp": "2026-10-18T21:43:20.243411106Z",
      "usageCounter": 53
    },
    "SparksSong:sid_placeholder_753": {
      "lastUsedTimestamp": "2026-10-18T21:43:20.243411106Z",
      "usageCounter": 53
    },
    "VehicleCosmetics_Body:id_body_squash": {
      "lastUsedTimestamp": "2026-10-18T21:43:20.243411106Z",
      "usageCounter": 53
    },
    "VehicleCosmetics_Booster:id_booster_slimefire": {
      "lastUsedTimestamp": "2026-10-18T21:43:20.243411106Z",
      "usageCounter": 53
    },
    "VehicleCosmetics_DriftTrail:id_drifttrail_cybersecurity": {
      "lastUsedTimestamp": "2026-10-18T21:43:20.243411106Z",
      "usageCounter": 53
    },
    "VehicleCosmetics_Skin:carskin_squashaventurine01": {
      "lastUsedTimestamp": "2026-10-18T21:43:20.243411106Z",
      "usageCounter": 53
    },
    "VehicleCosmetics_Wheel:wheel_petal4": {
      "lastUsedTimestamp": "2026-10-18T21:43:20.243411106Z",
      "usageCounter": 53
    }
  }
}
```
