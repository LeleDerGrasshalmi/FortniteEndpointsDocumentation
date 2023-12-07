## Wasp Service - Generate World Token (For MMS)

URL: https://wasp-service-live-public.ogs.live.on.epicgames.com/api/v1/namespace/:namespaceId/worlds/world/:worldId/attest/:accountId \
Method: GET \
Auth Required: Yes (`wasp:{namespaceId}:world READ`)

## Path Parameters

`namespaceId`: Check [Readme](../README.md) <br/>
`worldId` The World Id from the [worlds list](./AccountAccessibleWorld.md) <br/>
`accountId`: Your Account Id

---

_Example Response_

This Plain JWT Token must be included inside the `player.option.worldIdToken` mms ticket param.

```
wasp~eyJraWQiOiJhdHRlc3QxIiwidHlwIjoiSldUIiwiYWxnIjoiRWREU0EifQ.eyJhY2NvdW50SWQiOiI5NGIxNTY5NTA2YjA0ZjlmODU1N2FmNjExZThjNWU0NyIsIm5hbWVzcGFjZUlkIjoiZm4iLCJ3b3JsZElkIjoiODJhMGZhMzhhN2IyNDViY2E3MGJiNWY1MGJhOGQxOGUiLCJpc3MiOiJlcGljZ2FtZXMiLCJleHAiOjE3MDE2MjY0MjYsImlhdCI6MTcwMTYyNjEyNn0.JRjX2xD1JnIUGbXGlGdasGGhPcuZ6KdIWJSer_GCJBoAISws8grT10CIPplnzTMM8xujN1CqF4uCw5yx1NlhAA
```
