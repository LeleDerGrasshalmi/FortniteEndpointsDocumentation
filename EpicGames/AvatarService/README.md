# Avatar Service

Fortnite outfit avatars of accounts, used by the Epic Games social overlay (friends list, party, group chats). Every route takes the avatars deployment id `9c9906b240c74a92a6b9100d6e4ccbd0`. Requests need an account access token; an EOS token is rejected.

## Hosts

- api.epicgames.dev (path prefix `/epic/avatar`)
- avatars-service-prod.social.live.on.epicgames.com (older)

Avatar image URLs contain `{}`, replace it with the height in pixels.
