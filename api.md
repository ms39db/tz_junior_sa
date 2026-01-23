## Задача


Описание:
Интернет-магазин "Петрушка Зеленая" преуспевает, расширяется и в мобильном приложении решили создать новый экран, который будет отображать магазины партнеров (см. макеты ниже).

<img width="342" height="509" alt="Screenshot 2026-01-23 at 22 20 24" src="https://github.com/user-attachments/assets/843e1995-8368-4091-a56b-fd8a57fa9c44" />


Что нужно сделать:
Написать пример REST API запроса, который будет вызываться при переходе пользователя на данный экран. 
Привести пример ответа этого REST API в соответствии с макетом. Формат - JSON. Учесть, что при клике на плашку магазина должен осуществляться переход по ссылке на внешний ресурс. 


## Решение

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


