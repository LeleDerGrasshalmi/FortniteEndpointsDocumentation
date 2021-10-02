# Fortnite Related Endpoint Documentation
By jemcer#1009 &amp; LeleDerGrasshalm#1872

## Fortnite Website

this below is unkown if u need auth or not, since with bearer gives forbidden, but if logged in with browser works...
| Name | URL | Method | Auth Required | Body
| ----------- | ----------- | ----------- | ----------- | ----------- |
| Code Redeem (Title/Desc) | https://www.epicgames.com/fortnite/ajax/redemption/validate-redemption-code?redeem-code=XLKCH-6VLA2-9ZQAT-ZU85F | GET | Yes/No? idk | None
| Submit Code Redeem | https://www.epicgames.com/fortnite/ajax/redemption/submit-redemption-code | POST | Yes/No? idk | FormData: hotsPageId=code-redeem&redeem-code={Code}&locale=en
