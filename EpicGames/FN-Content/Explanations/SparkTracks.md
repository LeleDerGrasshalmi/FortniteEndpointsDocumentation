## FN - Content API - Spark Tracks (Jam Tracks) Structure

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
      "ry": 2021,
      "dn": 157,
      "sib": "Bass",
      "sid": "Drum",
      "sig": "Guitar",
      "qi": "{\"sid\":\"764abe5f-8530-42f3-b235-7661b2dc7c66\",\"pid\":\"ac07da2b-d589-4d96-b1a4-62a7be6cb47e\",\"stereoId\":\"5a52481b-092e-432a-a847-f3b43b4e0ec9\",\"instrumentalId\":\"e1ea6bc3-e790-44f8-a45a-9ed0b10f91a2\",\"title\":\"butterbarnhoedown\",\"tracks\":[{\"part\":\"ds\",\"channels\":[\"FL\",\"FR\"],\"vols\":[4,4]},{\"part\":\"bs\",\"channels\":[\"FL\",\"FR\"],\"vols\":[4,4]},{\"part\":\"gs\",\"channels\":[\"FL\",\"FR\"],\"vols\":[4,4]},{\"part\":\"vs\",\"channels\":[\"FL\",\"FR\"],\"vols\":[4,4]},{\"part\":\"fs\",\"channels\":[\"FL\",\"FR\"],\"vols\":[4,4]}],\"preview\":{\"starttime\":44.0816}}",
      "sn": "butterbarnhoedown",
      "ge": ["Country"],
      "mk": "D",
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
      "mt": 98,
      "_type": "SparkTrack",
      "mu": "https://cdn2.unrealengine.com/fkrvlnrmue22iamp-fa60196359dc.dat",
      "an": "Epic Games",
      "gt": ["Jam-LoopIsUnpitched-Beat"],
      "ar": "E",
      "au": "https://cdn2.unrealengine.com/8trfqm9nofp8xeoj-512x512-4d008e153456.jpg",
      "ti": "SparksSong:sid_placeholder_02",
      "ld": "https://cdn2.unrealengine.com/butterbarnhoedown-dea9cb878493.lad",
      "jc": "2966-7543-4422"
    },
    "_noIndex": false,
    "_activeDate": "2023-10-09T18:12:20.689Z",
    "lastModified": "2024-09-13T02:31:08.018Z",
    "_locale": "en-US",
    "_templateName": "track"
  },
  "_suggestedPrefetch": []
}
```

</details>

## Structure Explained

Each Track is a object in the root object, each `track` object has the following structure.

| Property             | Type     | Explanation                     |
| -------------------- | -------- | ------------------------------- |
| tt                   | string   | Track Title                     |
| ry                   | int      | Release Year                    |
| dn                   | int      | Duration (in seconds)           |
| sib                  | string   | Starting Instrument Bass        |
| sid                  | string   | Starting Instrument Drums       |
| sig                  | string   | Starting Instrument Guitar      |
| qi                   | string   | Quicksilver Data                |
| qi.sid               | string   | Song streaming UUID             |
| qi.pid               | string   | Preview streaming UUID          |
| qi.stereoId          | string   | Stereo streaming UUID           |
| qi.instrumentalId    | string   | Instrumental streaming UUID     |
| qi.title             | string   | Short song title                |
| qi.tracks            | object[] | Track Data                      |
| qi.preview           | object   | Preview Data                    |
| qi.preview.starttime | float    | Preview start time (in seconds) |
| sn                   | string   | Track Name for API              |
| ge                   | string[] | Song Genre                      |
| mk                   | string   | Key                             |
| mm                   | string   | Scale                           |
| ab                   | string   | Album Name                      |
| siv                  | string   | Starting Instrument Vocals      |
| su                   | string   | Event UUID                      |
| in                   | object   | Song Difficulties               |
| in.pb                | int      | Plastic Bass Difficulty         |
| in.pd                | int      | Plastic Drums Difficulty        |
| in.pg                | int      | Plastic Guitar Difficulty       |
| in.vl                | int      | Vocals Difficulty               |
| in.gr                | int      | Guitar Difficulty               |
| in.ds                | int      | Drums Difficulty                |
| in.ba                | int      | Bass Difficulty                 |
| mt                   | int      | BPM/Tempo                       |
| mu                   | string   | Encrypted MIDI Data URL         |
| an                   | string   | Artist Name                     |
| gt                   | string[] | Gameplay Tags                   |
| isrc                 | string   | ISR Code (ISRC)                 |
| ar                   | string   | ISRB Rating                     |
| au                   | string   | Album Art URL                   |
| ti                   | string   | Template ID                     |
| ld                   | string   | Lipsync Data URL                |
| jc                   | string   | Jam Link Code                   |
