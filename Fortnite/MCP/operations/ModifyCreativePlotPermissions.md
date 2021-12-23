# ModifyCreativePlotPermissions

**Description**: `Mofifies the Creative Island Permission for specified users` \
**Profiles**: `creative` \
**Note**: `DedicatedServer ONLY`

## Body
```js
{
    "plotItemId": "", //island/plot item (templateId or guid idk)
    "permission": "", //the permission to give the users, valid: Private & Public
    "accountIds": [] //array of the players accountId
}
```
