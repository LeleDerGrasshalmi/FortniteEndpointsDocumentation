## Nelly Service - Report

URL: https://nelly-service-prod.ecbc.live.use1a.on.epicgames.com/v1/report \
Method: POST \
Auth Required: No

> You can use any of the available provider hosts in the [README](README.md)

```json
{
  "source": "talon",
  "encountered_report_error": false,
  "results": {
    "direct_small_get": {
      "provider": "direct",
      "successful": true,
      "performance": {
        "e2e": 1139
      }
    },
    "cloudfront_small_get": {
      "provider": "cloudfront",
      "successful": true,
      "performance": {
        "e2e": 164
      }
    },
    "fastly_small_get": {
      "provider": "fastly",
      "successful": true,
      "performance": {
        "e2e": 92
      }
    },
    "akamai_small_get": {
      "provider": "akamai",
      "successful": true,
      "performance": {
        "e2e": 145
      }
    },
    "cloudflare_small_get": {
      "provider": "cloudflare",
      "successful": true,
      "performance": {
        "e2e": 178
      }
    }
  },
  "provider": "fastly"
}
```

## Parameters

`source`: What caused this task to be executed <br/>
`encountered_report_error`: Wheter whgat <br/>
`results`: A record of the Task Id and the Task result <br/>
`results[taskId].provider`: The provider that was used to execute the task <br/>
`results[taskId].successful`: If the task was successful <br/>
`results[taskId].performance`: Performance stats for this task execution <br/>
`results[taskId].performance.e2e`: The time in ms that it took for the task to complete (end to end) <br/>
`provider`: Which provider host was used to receive the tasks and used to report the results

---

_Example Response_: Status 204
