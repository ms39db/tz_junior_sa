## GET

### Request

GET /api/delivery

url: https://petrushka.ru/api/delivery?address=ул+ленина+67

headers:

content-type: application/json


### Response

status: 200

headers:
content-type: application/json

body:
```json
{
  "status": "ok",
  "address": "ул Ленина 67",
  "data": [ 
      {
        "name": "metro",
        "logo": "string",
        "url": "string",
        "delivery_time": {
          "fast_delivery": false,
          "delivery_time_frrom": "2026-01-22T21:00:00",
          "delivery_time_to": "2026-01-22T23:00:00"
        }
      },
      {
        "name": "ashan",
        "logo": "string",
        "url": "string",
        "delivery_time": {
          "fast_delivery": false,
          "delivery_time_frrom": "2026-01-22T19:00:00",
          "delivery_time_to": "2026-01-22T20:00:00"
        }
      },
      {
        "name": "vkusvill",
        "logo": "string",
        "url": "string",
        "delivery_time": {
          "fast_delivery": true,
          "min_time": 20,
          "max_time": 60
        }
      },
      {
        "name": "viktoria",
        "logo": "string",
        "url": "string",
        "delivery_time": {
          "fast_delivery": false,
          "delivery_time_frrom": "2026-01-22T17:00:00",
          "delivery_time_to": "2026-01-22T19:00:00"
        }
      }
    ]
}


