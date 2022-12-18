## Events Service - Events List (Data)

URL: https://events-public-service-live.ol.epicgames.com/api/v1/events/:GameId/download/:AccountId?region=EU&platform=Windows&teamAccountIds=xxx,yyy,zzz \
Method: GET \
Auth Required: Yes

### Parameter

`GameId`: Fortnite

`region`: e.g. EU \
`platform`: e.g. Windows \
`teamAccountIds`: Account Ids seperated by a comma ','

<br/>

## Events Service - Events List (Download)

URL: https://events-public-service-live.ol.epicgames.com/api/v1/events/:GameId/data/:AccountId?region=EU&showPastEvents=true&showPrivateEvents=false \
Method: GET \
Auth Required: Yes

### Parameter

`GameId`: Fortnite

`region`: e.g. EU (if not specified shows for all regions!) \
`showPastEvents`: true \
`showPrivateEvents`: false (throws because you dont have access!)
