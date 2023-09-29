## UE Marketplace - Review Detail

URL: https://www.unrealengine.com/marketplace/api/review/:offerId/:type/detail \
Method: GET \
Auth Required: Yes

## Path Parameters

`offerId`: The Id of the Offer <br/>
`type`: The Type of the review (reviews,questions,replies)

---

_Example Response_

```json
{
  "status": "OK",
  "data": {
    "elements": [
      {
        "displayed": true,
        "id": "8cebaea55cb74abf854171c0a4a3d64d",
        "title": "Questions about animations",
        "identityId": "8752c28483cb4704baa4de1413ce84fd",
        "namespace": "ue",
        "storeName": "UES",
        "targetId": "a3d91055eb4b475ebe9ce9c60dd682a9",
        "targetOwner": "db66ba44fd8342548784e8c836064112",
        "content": "<p>Hello, Does this asset come with the animations seen in the youtube video?</p><p>Do you have those animations for the Unity version?</p><p>Thank you :)</p>",
        "status": "ACTIVE",
        "createdAt": "2023-07-17T04:31:12.708+0000",
        "lastModifiedAt": "2023-07-17T04:31:12.708+0000",
        "publisherReply": {
          "displayed": true,
          "id": "85fc6d33f12045cf8b2c32e55f319359",
          "identityId": "db66ba44fd8342548784e8c836064112",
          "topicId": "8cebaea55cb74abf854171c0a4a3d64d",
          "topicType": "QUESTION",
          "content": "<p>Hi! This asset comes with standard ue5 animations. </p><p>Unity project does not contain these animations because they are owned by Unreal Engine. This character has humanoid rig and you can use any animations from the store. However, I cannot help you with Unreal to Unity animations migration because I’ve never done it before. In theory, you can apply animations in Unreal engine and then export it as fbx. You can import this file to Unity. But again, I’ve never done it before so it’s just an assumption of what can be done.</p>",
          "isBest": false,
          "helpfulNum": 0,
          "status": "ACTIVE",
          "createdAt": "2023-07-17T10:33:03.609+0000",
          "lastModifiedAt": "2023-07-17T10:33:03.609+0000",
          "alreadyUpvote": false,
          "identityName": "IdaFaber",
          "isCurrentUser": false,
          "identityOwned": true
        },
        "alreadyUpvote": false,
        "helpfulNum": 0,
        "replyNum": 1,
        "bestAnswerSeleted": false,
        "identityName": "HamsterHam33",
        "isCurrentUser": false,
        "identityOwned": false
      }
    ],
    "paging": {
      "count": 10,
      "start": 0,
      "total": 2
    }
  }
}
```
