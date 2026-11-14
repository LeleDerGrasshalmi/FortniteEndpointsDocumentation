# Library Service

## Hosts

- library-service.live.use1a.on.epicgames.com
- distro-gateway-prod.ol.epicgames.com

Both hosts serve the same paths (`/library/api/public/...`) and return the same responses. The Epic Games Launcher switched to `distro-gateway-prod.ol.epicgames.com` in November 2026.

## Obtaining the Artifact Id

1. Lookup the Catalog Item
2. Get the `appId` of the Catalog Item inside `releaseInfo`

> e.g. `963137e4c29d4c79a81323b8fab03a40` for Among Us (Namespace: `33956bcb55d4452d8c47e16b94e294bd`, ItemId: `729a86a5146640a2ace9e8c595414c56`)
