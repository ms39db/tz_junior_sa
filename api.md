## GET

### Request

Method GET
url: "string"
host: "string"

headers:
conten-type: application/json

body:
```json
{
  "address": "string"
}
```

### Response

status: 200

headers:
conten-type: application/json

body:
```json
{
  "status": "ok",
  "address": "string",
  "data": [ 
      {
        "name": "Metro",
        "logo": "string",
        "url": "string",
        "fast_delivery": false,
        "delivert_time": "timestamp"
      },
      {
        "name": "ashan",
        "logo": "string",
        "url": "string",
        "fast_delivery": false,
        "delivert_time": "timestamp"
      },
      {
        "name": "vkusvill",
        "logo": "string",
        "url": "string",
        "fast_delivery": false,
        "delivert_time": "timestamp"
      },
      {
        "name": "viktoria",
        "logo": "string",
        "url": "string",
        "fast_delivery": false,
        "delivert_time": "timestamp"
      }
    ]
}


