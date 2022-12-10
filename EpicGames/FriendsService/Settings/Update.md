## Friends Service - Update Privacy Settings

URL: https://friends-public-service-prod.ol.epicgames.com/friends/api/v1/:accountId/settings \
Method: PATCH \
Auth Required: Yes

```js
{
    "acceptInvites": "public", // public, private
    "mutualPrivacy": "ALL" // ALL, FRIENDS, NONE
}
```

### **RELICT**

The Method orginally was **PUT** but **now** is PATCH, PUT is a relict, it only updates the acceptInvites setting. <br/>
Even if both settings are required in the body, likely cause by the same requet model, instead of fixing the PUT they just added PATCH and use that now.
