## Emerald Service - Upload: Init

URL: https://emerald-service-live.ecosec.on.epicgames.com/emerald/v1/upload/init \
Method: POST \
Auth Required: Yes (`emerald:upload CREATE`)

---

_Example Response_

```json
{
  "token": "VjF7ImMiOiJtdS12b2ljZS1tb2RlcmF0aW9uLWxpdmUiLCJ1IjpbeyJpIjoiIiwiZCI6InMzOi8vcHJvZC11c3cyLXJ0Y3AtbW9kZXJhdGlvbi11cGxvYWRzL3ZvaWNlLW1vZGVyYXRpb24tbGl2ZS81MTc5MzBjMC0xYTRlLTRmMWUtYjFhMi1mNGM5NzQ0Y2Y0YWIvcmVjb3JkaW5nLmJpbiIsImYiOiJyZWNvcmRpbmcuYmluIn1dfQ==",
  "files": {
    "recording.bin": {
      "chunkUrls": [
        "https://prod-usw2-rtcp-moderation-uploads.s3.us-west-2.amazonaws.com/voice-moderation-live/517930c0-1a4e-4f1e-b1a2-f4c9744cf4ab/recording.bin?X-Amz-Algorithm=XXX&X-Amz-Credential=XXX&X-Amz-Date=XXX&X-Amz-Expires=XXX&X-Amz-Security-Token=XXX&X-Amz-SignedHeaders=XXX&X-Amz-Signature=XXX"
      ]
    }
  }
}
```
