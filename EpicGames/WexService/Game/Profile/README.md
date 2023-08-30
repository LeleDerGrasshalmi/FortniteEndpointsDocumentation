# Battle Breakers MCP Profile Operations

## Request

**Method**: `POST` \
**URL**: `https://wex-public-service-live-prod.ol.epicgames.com/wex/api/game/v2/profile/:accountId/:operation` \
**Body**: `Individual`

## Query Parameters

| Name      | Value       | Default Value |
| --------- | ----------- | ------------- |
| profileId | {profileId} | profile0      |
| rvn       | -1          | -1            |

<br/>

## Profiles

| ProfileId   | Description                                                            |
| ----------- | ---------------------------------------------------------------------- |
| profile0    | Main Profile Data (like "common_core" for Fortnite)                    |
| levels      | Completed Levels, Unlocked Zones, Claimed Territories, Personal Events |
| friends     | BB Specific Friend Data (Epic didn't use Friends Service until later)  |
| monsterpit  | Monster Pit Heroes + Pets (like Collection Book)                       |
| multiplayer | PVP Data (Opponents, stats, history)                                   |
