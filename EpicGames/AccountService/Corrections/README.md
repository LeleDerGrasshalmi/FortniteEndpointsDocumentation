# Error Response

When an corrective action is required, you will get such an error response when authenticating.

```json
{
  "errorCode": "errors.com.epicgames.oauth.corrective_action_required",
  "errorMessage": "Corrective action is required to continue.",
  "messageVars": [],
  "numericErrorCode": 18206,
  "originatingService": "com.epicgames.account.public",
  "intent": "prod",
  "continuation": "00000000000000000000000000000000",
  "continuationUrl": "https://epicgames.com/continue/00000000",
  "correctiveAction": "DATE_OF_BIRTH"
}
```

Known `correctiveAction` values:

- `CONFIRM_DISPLAY_NAME`, see [confirmDisplayName](./ConfirmDisplayName.md)
- `DATE_OF_BIRTH`, see [dateOfBirth](./DateOfBirth.md)
- `EULA_ACCEPTANCE`, see [acceptEula](./AcceptEula.md)
- `EXTERNAL_AUTH_NOT_FOUND`
- `GUARDIAN_EMAIL`, see [guardianEmail](./GuardianEmail.md)
- `LINK_REAL_ID`
- `PENDING_DELETION`, see [cancelPendingDeletion](./CancelPendingDeletion.md)
- `PRIVACY_POLICY_ACCEPTANCE`, see [acceptPrivacyPolicy](./AcceptPrivacyPolicy.md)
- `PROMOTE_ACCOUNT`, see [promoteAccount](./PromoteAccount.md)
- `SCOPE_CONSENT`
- `SUPPLEMENTAL_CONSENT`
