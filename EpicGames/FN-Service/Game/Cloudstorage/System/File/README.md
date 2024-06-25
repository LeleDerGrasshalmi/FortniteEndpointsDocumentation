# Restricted Files

There are restricted System Files, examples for those are the Dedicated Server hotfixes.

---

Back then you used to get a permission error like the following:

```json
{
  "errorCode": "errors.com.epicgames.common.missing_permission",
  "errorMessage": "Sorry your login does not posses the permissions 'fortnite:cloudstorage:system:DedicatedServerEngine.ini READ' needed to perform the requested operation",
  "messageVars": [
    "fortnite:cloudstorage:system:DedicatedServerEngine.ini",
    "READ"
  ],
  "numericErrorCode": 1023,
  "originatingService": "fortnite",
  "intent": "prod-live"
}
```

But at some point epic decided to add a own error, which doesnt expose the permission (filename) anymore:

```json
{
  "errorCode": "errors.com.epicgames.modules.cloudstorage.file_restricted",
  "errorMessage": "This client does not have permission to read that system file.",
  "messageVars": [],
  "numericErrorCode": -1,
  "originatingService": "fortnite",
  "intent": "prod-live"
}
```
