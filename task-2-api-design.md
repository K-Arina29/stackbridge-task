# Задание 2. Проектирование API

## 1. Пример REST API запроса

```http
GET /api/v1/delivery/stores?city_id=1 HTTP/1.1
Host: api.petrushkazelenaya.ru
Authorization: Bearer [token]
Accept: application/json

## 2. Пример ответа (JSON)
{
  "success": true,
  "timestamp": "2026-07-13T13:05:00Z",
  "data": [
    {
      "id": "metro_001",
      "name": "METRO",
      "logo_url": "https://storage.petrushka.ru/logos/metro.png",
      "delivery_info": "Ближайшая доставка сегодня 21:00-23:00",
      "delivery_time": "21:00-23:00",
      "external_link": "https://metro.ru/partner/petrushka?store=001",
      "is_available": true
    },
    {
      "id": "ashan_002",
      "name": "Ашан",
      "logo_url": "https://storage.petrushka.ru/logos/ashan.png",
      "delivery_info": "Ближайшая доставка сегодня 18:00-20:00",
      "delivery_time": "18:00-20:00",
      "external_link": "https://ashan.ru/petrushka?store=002",
      "is_available": true
    },
    {
      "id": "vkusvill_003",
      "name": "ВкусВилл",
      "logo_url": "https://storage.petrushka.ru/logos/vkusvill.png",
      "delivery_info": "Быстрая доставка от 20 до 60 минут",
      "delivery_time": "20-60 мин",
      "external_link": "https://vkusvill.ru/petrushka?store=003",
      "is_available": true
    }
  ]
}
