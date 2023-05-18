## Fortnite - Mobile Item Shop Assets (deprecated)

URL: https://www.epicgames.com/graphql \
Method: POST \
Auth Required: No

```json
{
  "query": "query FortniteQuery { Fortnite { getCurrentStoreOffers { storefronts { catalogEntries { offerId devName assetName } } success } } }"
}
```

---

_Example Response (shortened)_

```json
{
  "data": {
    "Fortnite": {
      "getCurrentStoreOffers": {
        "storefronts": [
          {
            "catalogEntries": [
              {
                "offerId": "v2:/2cccc4c4c393a0d1438f41a4d7e60bbac9cde165f37be73cee93c0827586b718",
                "devName": "[VIRTUAL]1 x Fishy for 300 MtxCurrency",
                "assetName": "wrap_073_44056076ba52c7785ff0774683a84e70ea2e1fd32ce267b88e15ae3198e26060.jpg"
              },
              {
                "offerId": "v2:/f5bba5bee19d45adfbed1a8b33069aed95e5cc30f87dbe2f117871ab60e58697",
                "devName": "[VIRTUAL]1 x Coral Cruiser for 800 MtxCurrency",
                "assetName": "glider_id_c605061406b82169f659965dfde22028c7d51e7fb660219ef930413a143832fd.jpg"
              }
            ]
          },
          {
            "catalogEntries": [
              {
                "offerId": "v2:/219e96eaf84ef6c2dfc984cda537c592ffd132993fb76777e1a68c1c04486aad",
                "devName": "[VIRTUAL]1 x Astra, 1 x Shining Star for 1500 MtxCurrency",
                "assetName": "cid_642_cbf70778902258c427d989e0c7b518ff43c2444dc43da2a6bde396d521e37925.jpg"
              }
            ]
          }
        ],
        "success": true
      }
    }
  },
  "extensions": {}
}
```

---

_Requesting the Image_

GET `https://cdn2.unrealengine.com/Kairos/itemShopAssets/:assetName` <br/>
e.g. `https://cdn2.unrealengine.com/Kairos/itemShopAssets/cid_642_cbf70778902258c427d989e0c7b518ff43c2444dc43da2a6bde396d521e37925.jpg`

<img src="https://cdn2.unrealengine.com/Kairos/itemShopAssets/cid_642_cbf70778902258c427d989e0c7b518ff43c2444dc43da2a6bde396d521e37925.jpg" width="25%">
