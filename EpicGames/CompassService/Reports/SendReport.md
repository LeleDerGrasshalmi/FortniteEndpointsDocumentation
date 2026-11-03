## Compass Service - Reports: Send Report

URL: https://compass-service-prod.ecosec.on.epicgames.com/compass/v1/namespace/eos/new_social_overlay_report Method: POST Auth Required: Yes (Account Auth)

```json
{
  "reporter_entity_id": "94b1569506b04f9f8557af611e8c5e47",
  "offender_entity_id": "07c0ExampleGroupId0008",
  "reason": "group.chat",
  "emerald_token": "3e7b1c9d-5a2f-4d8e-b6c0-1f4a7e9d2b3c"
}
```

## Parameters

`reporter_entity_id`: Your AccountId <br/>
`offender_entity_id`: The Conversation Id of the reported group chat <br/>
`reason`: `group.chat` <br/>
`emerald_token`: The `token` returned by [Emerald Service Upload Text](../../EmeraldService/Upload/UploadText.md)

---

_Example Response_

```json
{
  "report_id": "9c2e4a6b-8d1f-4e3a-b5c7-0a2d4f6e8b1c",
  "product_id": "social_overlay",
  "report_reason": "terms_of_service",
  "report_state": "Pending Moderation",
  "report_status": "open",
  "creation_datetime": "2026-10-15T02:05:23.239987559Z",
  "last_updated": "2026-10-15T02:05:23.239987559Z",
  "reporter_entity_type": "epic_account",
  "offender_entity_type": "epic_account",
  "appealed": false,
  "actioned": false,
  "moderation_type": "badger",
  "product_report_type": "group.chat",
  "history": [
    {
      "id": "1a3c5e7f-9b2d-4f6a-8c0e-4b6d8f0a2c3e",
      "created_at": "2026-10-15T02:05:23.243171955Z",
      "updated_at": "2026-10-15T02:05:23.243196108Z",
      "report_id": "9c2e4a6b-8d1f-4e3a-b5c7-0a2d4f6e8b1c",
      "event": "created"
    }
  ],
  "can_appeal": false,
  "appeal_unavailable_reason": "report_open",
  "has_sanction": false
}
```
