## Friends Service - Edit Alias

URL: https://friends-public-service-prod.ol.epicgames.com/friends/api/v1/:accountId/friends/:friendId/alias \
Method: PUT \
Auth Required: Yes (`friends:{accountId} UPDATE`)

## Headers

`Content-Type`: text/plain

---

_The body is the new alias (min 3, max 16 characters)_

```
lele test
```

## Path Parameters

`accountId`: Your Account Id <br/>
`friendId`: Friend Account Id

---

_Example Response_: Status 204

_Example Response (invalid alias)_

```json
{
  "errorCode": "errors.com.epicgames.validation.validation_failed",
  "errorMessage": "Validation Failed. Invalid fields were [alias]",
  "messageVars": ["[alias]"],
  "numericErrorCode": 1040,
  "originatingService": "friends",
  "intent": "prod",
  "validationFailures": {
    "alias": {
      "fieldName": "alias",
      "errorMessage": "Incorrect alias input. Should be from 3 to 16 letters, digits, spaces, -, _, . or emoji.",
      "errorCode": "com.epicgames.friends.validation.constraints.alias",
      "invalidValue": "invalid ###",
      "messageVars": {
        "pattern": "[\\p{LD} \\-_.'‘’]+",
        "maxSize": "16",
        "minSize": "3"
      }
    }
  }
}
```
