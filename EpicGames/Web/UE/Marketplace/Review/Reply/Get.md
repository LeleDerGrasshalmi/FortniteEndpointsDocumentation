## UE Marketplace - Get

URL: https://www.unrealengine.com/marketplace/api/review/:type/:topicId/reply \
Method: GET \
Auth Required: Yes

### Query Parameters

**start**: The Start number you want to view
**count**: Total Count Per Page
**offerId** the Id of the Offer

## Path Parameters

`type`: the Type of the review (reviews,questions,replies)
`topicId`: the TopicId of the review

---

_Example Response_

```json
{
    "elements": [
        {
            "displayed": true,
            "id": "",
            "identityId": "",
            "topicId": "",
            "topicType": "REVIEW",
            "content": "<p>test</p>",
            "isBest": false,
            "helpfulNum": 0,
            "status": "ACTIVE",
            "createdAt": "2023-08-26T17:27:02.704+0000",
            "lastModifiedAt": "2023-08-26T17:27:02.704+0000",
            "alreadyUpvote": false,
            "storeName": "UES",
            "namespace": "ue",
            "identityName": "test",
            "isCurrentUser": true,
            "identityOwned": true
        }
    ],
    "paging": {
        "count": 10,
        "start": 0,
        "total": 1
    }
}
```