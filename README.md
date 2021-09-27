# Fortnite Related Endpont Documentation
By jemcer#1009 &amp; LeleDerGrasshalm#1872

## Epic Games Store

| Name | URL | Method | Auth Required | Body
| ----------- | ----------- | ----------- | ----------- | ----------- |
| Site | https://store-content.ak.epicgames.com/api/en-US/content/products/fortnite | GET | No | None

## Fortnite

| Name | URL | Method | Auth Required | Body
| ----------- | ----------- | ----------- | ----------- | ----------- |
| Content | https://fortnitecontent-website-prod07.ol.epicgames.com/content/api/pages/fortnite-game | GET | No | None
| Calendar/Timeline | https://fortnite-public-service-prod11.ol.epicgames.com/fortnite/api/calendar/v1/timeline | GET | YES | None
| Keychain | https://fortnite-public-service-prod11.ol.epicgames.com/fortnite/api/storefront/v2/keychain | GET | YES | None
| Catalog/Store | https://fortnite-public-service-prod11.ol.epicgames.com/fortnite/api/storefront/v2/catalog | GET | YES | None
| Info for AppstoreId(s) | https://catalog-public-service-prod06.ol.epicgames.com/catalog/api/shared/bulk/offers?id={AppstoreId} | GET | YES | None
| Server Status | https://lightswitch-public-service-prod06.ol.epicgames.com/lightswitch/api/service/bulk/status?serviceId=Fortnite | GET | YES | None
| Manifest - Windows | https://launcher-public-service-prod06.ol.epicgames.com/launcher/api/public/assets/v2/platform/Windows/namespace/fn/catalogItem/4fe75bbc5a674f4f9b356b5c90567da5/app/Fortnite/label/Live | GET | YES | None
| Manifest - Android | https://launcher-public-service-prod-m.ol.epicgames.com/launcher/api/public/assets/Android/5cb97847cee34581afdbc445400e2f77/FortniteContentBuilds?label=Live | GET | YES | None
| Manifest - IOS | https://launcher-public-service-prod06.ol.epicgames.com/launcher/api/public/assets/IOS/5cb97847cee34581afdbc445400e2f77/FortniteContentBuilds?label=Live | GET | YES | None
