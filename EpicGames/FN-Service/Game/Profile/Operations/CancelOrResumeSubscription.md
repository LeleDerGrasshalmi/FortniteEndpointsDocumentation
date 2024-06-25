# CancelOrResumeSubscription

**Description**: `Cancels or Continues a Subscription (e.g. Fortnite Crew)` \
**Profiles**: `common_core`

## Body

```js
{
    "appStore": "", // App Store that the Subscription belongs to (from profile), e.g. EpicPurchasingService
    "uniqueSubscriptionId": "", // Subcription Id (from profile)
    "willAutoRenew": false
}
```
