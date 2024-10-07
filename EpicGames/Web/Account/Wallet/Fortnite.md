## Account Web - Wllet: Fortnite

URL: https://www.epicgames.com/account/v2/api/wallet/fortnite \
Method: GET \
Auth Required: Yes

---

_Example Response_

```json
{
  "success": true,
  "message": "",
  "data": {
    "Purchased": {
      "title": "epic.account.management.in_game_currency.purchased.table.title",
      "subtitle": "epic.account.management.in_game_currency.purchased.table.subtitle",
      "columns": [
        {
          "key": "Switch",
          "title": "epic.account.management.in_game_currency.group.nintendo"
        },
        {
          "key": "Shared",
          "title": "epic.account.management.in_game_currency.group.shared",
          "tooltip": "epic.account.management.in_game_currency.group.shared.tooltip"
        }
      ],
      "rows": {
        "Currency:MtxPurchased": {
          "title": "epic.account.management.in_game_currency.purchased.paid",
          "Switch": 0,
          "Shared": 350
        },
        "Currency:MtxPurchaseBonus": {
          "title": "epic.account.management.in_game_currency.purchased.bonus",
          "Switch": 0,
          "Shared": 0
        }
      }
    },
    "Earned": {
      "title": "epic.account.management.in_game_currency.earned.table.title",
      "subtitle": "epic.account.management.in_game_currency.earned.table.subtitle",
      "rows": [
        {
          "title": "epic.account.management.in_game_currency.earned.table.row.title",
          "value": 0
        }
      ]
    }
  },
  "lastUpdated": 1695361387285
}
```
