# CompletePlayerSurvey

**Description**: `Marks a Player Survey as completed` \
**Profiles**: `common_core`

## Body

```js
{
    "surveyId": "", // See below
    "bUpdateAllSurveysMetadata": true // If the survey_data.allSurveysMetadata should update
}
```

### Survey Id

- Examples:

  - 220320_Overall Health_FNC
  - 210504_Building_FNBR
  - 10504_Heartbeat Satisfaction_FNBR

- Obtaining:
  - Survey Data is stored in the [FN Content API](../../Content.md)
