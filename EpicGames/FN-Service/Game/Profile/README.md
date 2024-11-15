# Fortnite MCP Operations

## Request

**Method**: `POST` \
**URL**: `https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/game/v2/profile/:accountId/:route/:operation` \
**Body**: `Individual`

## Query Parameters

| Name      | Value       | Default Value |
| --------- | ----------- | ------------- |
| profileId | {profileId} | common_core   |
| rvn       | -1          | -1            |

**NOTE**: if its a "DedicatedServer ONLY" operation you cant use it

<br/>

## Profiles

| ProfileId                   | Description                                                                                                                                  |
| --------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| athena                      | Battle Royale data                                                                                                                           |
| creative                    | Creative data                                                                                                                                |
| campaign                    | Save the World data                                                                                                                          |
| common_public               | Public data (e.g. current user banner)                                                                                                       |
| collections                 | Battle Royale Collection (Fishing / NPC)                                                                                                     |
| common_core                 | Main Profile storing general info like banners, purchases, ban status & history, gift history and much more                                  |
| metadata                    | Save the World Homebase data (e.g info about user permission)                                                                                |
| collection_book_people0     | Collectionbook data (Heroes, Survivor, Defender)                                                                                             |
| collection_book_schematics0 | Collectionbook data (Schematics)                                                                                                             |
| outpost0                    | StW Storage                                                                                                                                  |
| theater0                    | StW Backpack                                                                                                                                 |
| theater1                    | Events Backpack (e.g. Frostnite, Hit the Road etc...)                                                                                        |
| theater2                    | Ventures data                                                                                                                                |
| recycle_bin                 | Stw Recycle Bin                                                                                                                              |
| proto_juno                  | Relict that doesnt exist anymore, was related to `ProtoJuno_*` Operations, relict from lego testing (now its a own service, not mcp related) |
| profile0                    | Relict that doesnt exist anymore since a long time, basicly like common_core, athena and campaign combined                                   |

<br/>

## Routes

| ProfileId        | Description                                                                                           |
| ---------------- | ----------------------------------------------------------------------------------------------------- |
| client           | The one you usually use                                                                               |
| public           | Only used for [QueryPublicProfile](./Operations/QueryPublicProfile.md)                                |
| dedicated_server | Server Route, requires `fortnite:fortnite_role:dedicated_server ALL` Permission (aka you cant use it) |
