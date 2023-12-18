# Spark Tracks (Jam Tracks) Structure

The `spark-tracks` sub-page has a heavily shortened structure as shown below.

<details>
  <summary>Open Structure Example</summary>

```json
{
  "_title": "spark-tracks",
  "_noIndex": false,
  "_activeDate": "2023-10-06T04:15:09.015Z",
  "lastModified": "2023-12-11T19:48:13.656Z",
  "_locale": "en-US",
  "_templateName": "blank",
  "butterbarnhoedown": {
    "_title": "butterbarnhoedown",
    "track": {
      "tt": "Butter Barn Hoedown",
      "mm": "Major",
      "ab": "Fortnite",
      "siv": "Vocals",
      "su": "6610181f-8c9f-46a4-82d1-b4a44bad9310",
      "in": {
        "pb": 2,
        "pd": 1,
        "vl": 4,
        "pg": 4,
        "_type": "SparkTrackIntensities",
        "gr": 4,
        "ds": 2,
        "ba": 1
      },
      "ry": 2021,
      "mt": 98,
      "_type": "SparkTrack",
      "mu": "https://cdn2.unrealengine.com/fkrvlnrmue22iamp-fa60196359dc.dat",
      "dn": 157,
      "sib": "Bass",
      "an": "Epic Games",
      "gt": ["Jam-LoopIsUnpitched-Beat"],
      "sid": "Drum",
      "sig": "Guitar",
      "au": "https://cdn2.unrealengine.com/8trfqm9nofp8xeoj-512x512-93503ff352b2.png",
      "ti": "SparksSong:sid_placeholder_02",
      "qi": "{\"sid\":\"bf582ade-70ac-4c56-be34-cb26f768c2c9\",\"pid\":\"049f79c3-8af5-4355-ba81-7d273850ad89\",\"title\":\"butterbarnhoedown\",\"tracks\":[{\"part\":\"ds\",\"channels\":[\"FL\",\"FR\"],\"vols\":[4,4]},{\"part\":\"bs\",\"channels\":[\"FL\",\"FR\"],\"vols\":[4,4]},{\"part\":\"gs\",\"channels\":[\"FL\",\"FR\"],\"vols\":[4,4]},{\"part\":\"vs\",\"channels\":[\"FL\",\"FR\"],\"vols\":[4,4]},{\"part\":\"fs\",\"channels\":[\"FL\",\"FR\"],\"vols\":[4,4]}],\"preview\":{\"starttime\":44.0816}}",
      "ld": "https://cdn2.unrealengine.com/butterbarnhoedown-dea9cb878493.lad",
      "jc": "2966-7543-4422",
      "sn": "butterbarnhoedown",
      "ge": ["Country"],
      "mk": "D"
    },
    "_noIndex": false,
    "_activeDate": "2023-10-09T18:12:20.689Z",
    "lastModified": "2023-12-05T22:07:18.035Z",
    "_locale": "en-US",
    "_templateName": "track"
  },
  "_suggestedPrefetch": []
}
```

</details>

## Structure Explained

Each Track is a object in the root object, each `track` object has the following structure.

| Property             | Type     | Explanaition                    |
| -------------------- | -------- | ------------------------------- |
| tt                   | string   | Track title                     |
| mm                   | string   |                                 |
| siv                  | string   |                                 |
| su                   | string   | Event UUID                      |
| in                   | object   |                                 |
| in.pb                | int      |                                 |
| in.pd                | int      |                                 |
| in.vl                | int      |                                 |
| in.pg                | int      |                                 |
| in.gr                | int      |                                 |
| in.ds                | int      |                                 |
| in.ba                | int      |                                 |
| ry                   | int      | Track Release Year              |
| mt                   | int      |                                 |
| mu                   | string   | binary data url                 |
| dn                   | int      |                                 |
| sib                  | string   |                                 |
| an                   | string   | Artist name                     |
| gt                   | string[] | Gameplay tags                   |
| sid                  | string   |                                 |
| sig                  | string   |                                 |
| au                   | string   | song icon url                   |
| ti                   | string   | Template Id                     |
| qi                   | string   | Stringified json object         |
| qi.sid               | string   | Song streaming UUID             |
| qi.pid               | string   | Preview streaming UUID          |
| qi.title             | string   | Short song title                |
| qi.tracks            | object[] | Track data                      |
| qi.preview           | object   | Preview data                    |
| qi.preview.starttime | float    | Preview start time (in seconds) |
| ld                   | string   | lipsync data url                |
| jc                   | string   | Join code (link code)           |
| sn                   | string   | Track Name for API              |
| ge                   | string[] | Song Genre                      |
| mk                   | string   |                                 |
