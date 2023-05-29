## IP-Data Service - Region

URL: https://ip-data-service-prod.ecbc.live.use1a.on.epicgames.com/region \
Method: GET \
Auth Required: Yes (`ipdata:region READ`)

---

_Example Response (shortened)_

```json
{
  "continent": {
    "code": "EU",
    "geoname_id": 6255148,
    "names": {
      "de": "Europa",
      "en": "Europe",
      "es": "Europa",
      "fr": "Europe",
      "ja": "ヨーロッパ",
      "pt-BR": "Europa",
      "ru": "Европа",
      "zh-CN": "欧洲"
    }
  },
  "country": {
    "geoname_id": 2921044,
    "is_in_european_union": true,
    "iso_code": "DE",
    "names": {
      "de": "Deutschland",
      "en": "Germany",
      "es": "Alemania",
      "fr": "Allemagne",
      "ja": "ドイツ連邦共和国",
      "pt-BR": "Alemanha",
      "ru": "ФРГ",
      "zh-CN": "德国"
    }
  },
  "subdivisions": [
    {
      "geoname_id": 2905330,
      "iso_code": "HE",
      "names": {
        "de": "Hessen",
        "en": "Hesse",
        "es": "Hessen",
        "fr": "Hesse",
        "ru": "Гессен"
      }
    }
  ]
}
```
