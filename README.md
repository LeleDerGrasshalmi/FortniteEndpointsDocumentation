# Epic Games - API ドキュメント

## 初めに


EpicGamesの多くのAPIには**認証**が必要です。アクセストークンを取得するには、[アクセストークン取得ガイド](./EpicGames/AccountService/Authentication/README.md#getting-started)　をご参照してください。
EpicGamesのAPIにリクエストするにはHTTPヘッダーにAuthorizationに、{bearer}:{アクセストークン}を指定する必要があります。

ただし、WebAPIには、クッキーが必要です。


## APIカテゴリ

- [Epic Games](./EpicGames)
  - [アカウントサービス](./EpicGames/AccountService)
  - [アーティファクトディスカバリー](./EpicGames/ArtifactDeliveryService)
  - [カルデラ](./EpicGames/CalderaService)
  - [データアセット](./EpicGames/DataAssetDirectoryService)
  - [プラットフォームAPI](./EpicGames/EGSPlatformService)
  - [エメラルドAPI](./EpicGames/EmeraldService)
  - [イベントサービス](./EpicGames/EventsService)
  - [フォートナイトサービス](./EpicGames/FN-Service)
  - [フォートナイトコンテンツAPI](./EpicGames/FN-Content)
  - [フォートナイトディスカバリー検索サービス](./EpicGames/FN-Discovery-Search-Service)
  - [フォートナイトランクAPI](./EpicGames/FN-Habanero-Service)
  - [フォートナイトホットコンフィグ](./EpicGames/FN-Hotconfig)
  - [フレンドサービス](./EpicGames/FriendsService)
  - [アクティブコード引き換えAPI](./EpicGames/FulfillmentService)
  - [言語設定...](./EpicGames/GlobalService)
  - [IPデータサービス](./EpicGames/IPDataService)
  - [KWS](./EpicGames/KWS)
  - [ランチャーサービスＡＰＩ](./EpicGames/LauncherService)
  - [各ゲームデータAPI](./EpicGames/LibraryService)
  - [ライトスイッチ（サーバーステータスAPI)](./EpicGames/LightswitchService)
  - [二モニック（プレイリスト）API](./EpicGames/LinksService)
  - [ネリーサービス](./EpicGames/NellyService)
  - [ディスプレイネーム検索サービス（利用不可）](./EpicGames/PersonaService)
  - [クリエイターマップ検索API](./EpicGames/PRMDialogService)
  - [ニュースフィードAPI](./EpicGames/StatsProxyService)
  - [タグ管理API](./EpicGames/TagManagementService)
  - [ユーザ検索](./EpicGames/UserSearchService)
  - [LEGO関連API](./EpicGames/WaspService)
  - [WexサービスAPI](./EpicGames/WexService)
  - [ウェブサービスAPI](./EpicGames/Web)
    - [アフィリエイト (SAC)](./EpicGames/Web/Affiliate)
    - [フォートナイト](./EpicGames/Web/Fortnite)
    - [Id](./EpicGames/Web/Id)
    - [アンリアルエンジン](./EpicGames/Web/UE)
      - [Marketplace](./EpicGames/Web/UE/Marketplace)
- [Epic Games Store](./EpicGamesStore)
- [Playstation Store](./PlaystationStore)



## ドキュメントの著者

- [Jem](https://twitter.com/jemfleaks) (jemcer#1009)
- [Lele](https://twitter.com/lel3x) (LeleDerGrasshalm#1872) - Most part
