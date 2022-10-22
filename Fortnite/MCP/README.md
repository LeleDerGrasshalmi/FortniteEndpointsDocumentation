# Fortnite MCP Operations

## Request

**Method**: `POST` \
**URL**: `https://fortnite-public-service-prod11.ol.epicgames.com/fortnite/api/game/v2/profile/:accountId/client/:operation` \
**Authorization Header**: `bearer {access_token}` \
**Body/Payload**: `individual for each operation` \
\
**Query Parameter:**

| Name      | Value       | Default Value |
| --------- | ----------- | ------------- |
| profileId | {profileId} | common_core   |
| rvn       | -1          | -1            |

**NOTE**: if its a "DedicatedServer ONLY" operation you cant use it

<br>

## Profiles

| ProfileId                   | Description                                                     |
| --------------------------- | --------------------------------------------------------------- |
| athena                      | Battle Royale data                                              |
| creative                    | Creative data                                                   |
| campaign                    | Save the World data                                             |
| common_public               | Public data (e.g. current user banner)                          |
| collections                 | Battle Royale Collection (Fishing / NPC)                        |
| common_core                 | here are banners saved, as well as other info like vbucks, etc. |
| metadata                    | saved which users have access on which homebase (StW)           |
| collection_book_people0     | Collectionbook data (Heroes, Survivor, Defender)                |
| collection_book_schematics0 | Collectionbook data (Schematics)                                |
| outpost0                    | StW Storage                                                     |
| theater0                    | StW Backpack                                                    |
| theater1                    | Events Backpack (e.g. Frostnite, Hit the Road etc...)           |
| theater2                    | Ventures data                                                   |
| recycle_bin                 | Stw Recycle Bin                                                 |
