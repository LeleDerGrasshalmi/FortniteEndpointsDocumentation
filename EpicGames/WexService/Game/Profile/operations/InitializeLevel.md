# InitializeLevel

**Description**: `Initializes and starts a level` \
**Profiles**: `levels`

## Body

```js
{
    "manifestVersion": "", // Client Content Version (body varies significantly between some versions)
    "levelId": "", // ID of Level to Initialize
    "partyMembers": [
        {
            "heroType": "", // Type of Party Member (e.g. LocalHero, FriendCommander)
            "heroItemId": "" // GUID of Hero
        }
    ],
    "friendInstanceId": "", // Friend Instance GUID (for friend commander)
    "ltmId": "", // ID of the active LTM for the zone
    "normalMode": true, // Challenge Mode
    "blitzMode": false, // Unused, blitz levels are not playable in later versions
    "teamPower": 364155 // Combined Hero Power
}
```
