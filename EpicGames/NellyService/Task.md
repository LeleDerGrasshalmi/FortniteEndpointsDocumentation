## Nelly Service - Task

URL: https://nelly-service-prod.ecbc.live.use1a.on.epicgames.com/v1/task \
Method: GET \
Auth Required: No

> You can use any of the available provider hosts in the [README](README.md)

---

_Example Response_

```json
{
  "sub_tasks": [
    {
      "task_id": "fastly_small_get",
      "provider": "fastly",
      "endpoint": "https://nelly-service-prod-fastly.ecosec.on.epicgames.com/v1/asset/fn_1k.jpeg"
    },
    {
      "task_id": "cloudflare_small_get",
      "provider": "cloudflare",
      "endpoint": "https://nelly-service-prod-cloudflare.ecosec.on.epicgames.com/v1/asset/fn_1k.jpeg"
    },
    {
      "task_id": "cloudfront_small_get",
      "provider": "cloudfront",
      "endpoint": "https://nelly-service-prod-cloudfront.ecosec.on.epicgames.com/v1/asset/fn_1k.jpeg"
    },
    {
      "task_id": "direct_small_get",
      "provider": "direct",
      "endpoint": "https://nelly-service-prod.ecbc.live.use1a.on.epicgames.com/v1/asset/fn_1k.jpeg"
    },
    {
      "task_id": "akamai_small_get",
      "provider": "akamai",
      "endpoint": "https://nelly-service-prod-akamai.ecosec.on.epicgames.com/v1/asset/fn_1k.jpeg"
    }
  ],
  "report_to": [
    {
      "task_id": "",
      "provider": "direct",
      "endpoint": "https://nelly-service-prod.ecbc.live.use1a.on.epicgames.com/v1/report"
    },
    {
      "task_id": "",
      "provider": "fastly",
      "endpoint": "https://nelly-service-prod-fastly.ecosec.on.epicgames.com/v1/report"
    },
    {
      "task_id": "",
      "provider": "cloudflare",
      "endpoint": "https://nelly-service-prod-cloudflare.ecosec.on.epicgames.com/v1/report"
    },
    {
      "task_id": "",
      "provider": "akamai",
      "endpoint": "https://nelly-service-prod-akamai.ecosec.on.epicgames.com/v1/report"
    },
    {
      "task_id": "",
      "provider": "cloudfront",
      "endpoint": "https://nelly-service-prod-cloudfront.ecosec.on.epicgames.com/v1/report"
    }
  ]
}
```
