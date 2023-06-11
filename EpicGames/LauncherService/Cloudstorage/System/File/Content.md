## Launcher Service - Cloudstorage: System File Content

URL: https://launcher-public-service-prod06.ol.epicgames.com/launcher/api/cloudstorage/system/:uniqueFilename \
Method: GET \
Auth Required: Yes (`launcher:cloudstorage:system:{uniqueFilename} READ`)

## Path Parameters

`uniqueFilename`: the `uniqueFilename` from the List

---

_Example Response (Fortnite.v2sdmeta)_

```json
{
  "DataType": "SelDlMeta",
  "Builds": [
    {
      "Namespace": "fn",
      "Item": "4fe75bbc5a674f4f9b356b5c90567da5",
      "Asset": "Fortnite",
      "Version": "Regex(\\+\\+Fortnite\\+Release-(.*)-CL-(\\d+)-.*) && RegexGroupInt64(2) < 4016789 && ((RegexGroupString(1) == \"Prep\" && RegexGroupInt64(2) >= 3779789) || (RegexGroupString(1) == \"Next\" && RegexGroupInt64(2) >= 3779794) || (RegexGroupString(1) == \"Cert\" && RegexGroupInt64(2) >= 3785892) || (RegexGroupInt64(2) >= 3846604))"
    }
  ],
  "Data": [
    {
      "Title": "Fortnite",
      "Title_translate": "true",
      "Description": "Files that are required to play the game.",
      "Description_translate": "true",
      "IsRequired": "true",
      "UniqueId": "3711A6568F844576B26E8CBB79EABC70",
      "Tags": ["", "chunk0", "chunk1"],
      "Title_fr": "Fortnite",
      "Description_fr": "Fichiers nécessaires pour jouer au jeu.",
      "Title_de": "Fortnite",
      "Description_de": "Benötigte Dateien, um das Spiel spielen zu können.",
      "Title_ru": "Fortnite",
      "Description_ru": "Обязательные файлы для запуска игры.",
      "Title_ko": "포트나이트",
      "Description_ko": "게임을 플레이하는 데 필요한 파일",
      "Title_tr": "Fortnite",
      "Description_tr": "Oyunu oynamak için gereken dosyalar.",
      "Title_it": "Fortnite",
      "Description_it": "I file che sono richiesti per giocare.",
      "Title_es": "Fortnite",
      "Description_es": "los archivos necesarios para jugar al juego.",
      "Title_es-MX": "Fortnite",
      "Description_es-MX": "Archivos necesarios para jugar el juego.",
      "Title_pl": "Fortnite",
      "Description_pl": "Pliki niezbędne do gry.",
      "Title_ar": "Fortnite",
      "Description_ar": "ملفات مطلوبة لبدء اللعبة.",
      "Title_ja": "フォートナイト",
      "Description_ja": "ゲームをプレイするために必要なファイル。",
      "Title_zh-CN": "《堡垒之夜》",
      "Description_zh-CN": "进行游戏需要的文件。",
      "Title_pt-BR": "Fortnite",
      "Description_pt-BR": "Arquivos necessários para jogar o Fortnite.",
      "Title_zh-Hans": "《堡垒之夜》",
      "Description_zh-Hans": "进行游戏需要的文件。",
      "Title_zh-Hant": "《Fortnite》",
      "Description_zh-Hant": "需要檔案才能進行遊戲。",
      "Title_th": "Fortnite",
      "Description_th": "ไฟล์ที่ต้องมีเพื่อเล่นเกม"
    }
  ]
}
```
