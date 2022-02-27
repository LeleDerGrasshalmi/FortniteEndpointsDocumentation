## Fortnite - BR News

URL: https://prm-dialogue-public-api-prod.edea.live.use1a.on.epicgames.com/api/v1/fortnite-br/surfaces/motd/target \
Method: POST \
Auth Required: Yes `(eg1)`

## Body
```json
{
   "platform": "Windows",
   "language": "en",
   "serverRegion": "EU",
   "country": "US",
   "subscription": false,
   "progressiveBackblingStage": 6,
   "CrewSep": true,
   "CrewOct": true,
   "CrewNov": true,
   "isRestricted": true,
   "totalHoursPlayed": 892,
   "seasonHoursPlayed": 592,
   "daysSinceLastSession": 1,
   "accountLevel": 593,
   "stylePoints": 333, 
   "globalCash": 0,
   "lifetimeWins": 84,
   "battlepass": true,
   "battlepassLevel": 225,
   "battlepassStars": 110,
   "battlepassItemsClaimed": 100,
   "bonusPage0Unlocked": true,
   "bonusPage1Unlocked": true,
   "unlockedPages": 15
}
```
`Replace the parameters with ur values, you can use none, specific or all of these parameter, depends on what you want (news are personalized)!`

<br>

Additional Parameter
```json
{
   "alienArtifacts": 222,
   "hasSavedEventDate": false,
   "hasAttendedEndOfSeasonS17": false,
   "MidSeasonS19": true,
   "hasMonarch": false,
   "hasShatteredWings": false,
   "hasMonarchGlow": false,
   "loneWolf": true,
   "loneWolfStyle": true,
   "buffLlama": true,
   "buffLlamaStyle": true,
   "islandNomad": true,
   "gumball": true,
   "gumballStyle": true,
   "motorcyclist": true,
   "spiderman": true,
   "spidermanStyle": true
}
```

NOTE: `The Parameter that are for current battle pass items change every season (listed in athenaseason{num})`
