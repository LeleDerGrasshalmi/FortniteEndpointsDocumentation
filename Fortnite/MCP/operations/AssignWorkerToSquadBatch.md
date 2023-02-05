# AssignWorkerToSquadBatch

**Description**: `Set an Gadget to an Loadout (Bulk)` \
**Profiles**: `campaign`

## Body

```js
{
    "characterIds": [], // The Survivor(Worker) Item GUIDs
    "squadIds": [], // The Squad Ids
    "slotIndices": [] // Slot within the Squads (0-7, 0 = Leader)
}
```

### Squad Id

- `Squad_Attribute_Medicine_EMTSquad` (EMT Squad)
- `Squad_Attribute_Arms_FireTeamAlpha` (Fire Team Alpha)
- `Squad_Attribute_Scavenging_Gadgeteers` (Gadgeteers)
- `Squad_Attribute_Synthesis_CorpsofEngineering` (Corps of Engineering)
- `Squad_Attribute_Medicine_TrainingTeam` (Training Team)
- `Squad_Attribute_Arms_CloseAssaultSquad` (Close Assault Squad)
- `Squad_Attribute_Scavenging_ScoutingParty` (Scouting Party)
- `Squad_Attribute_Synthesis_TheThinkTank` (The Think Tank)

<br/>

> Reference \
> `/SaveTheWorld/CommandConsole/CCSquads.uasset`
