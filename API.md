# Задание 2: проектирование API  
#### Описание:
Интернет-магазин "Петрушка Зеленая" преуспевает, расширяется и в мобильном приложении решили создать новый экран, который будет отображать магазины партнеров (см. макеты ниже).
![unnamed](https://github.com/user-attachments/assets/c0102d65-bb0e-48b2-8ec8-d440b9652c19)
#### Что нужно сделать:
Написать пример REST API запроса, который будет вызываться при переходе пользователя на данный экран. 
Привести пример ответа этого REST API в соответствии с макетом. Формат - JSON. Учесть, что при клике на плашку магазина должен осуществляться переход по ссылке на внешний ресурс. 

## Пример REST API запроса
GET /api/v1/partners
Accept: application/json

## Пример ответа REST API
{  
  "partners": [  
    {
      "id": 1,
      "name": "METRO",
      "delivery_info": "Ближайшая доставка сегодня 21:00–23:00",
      "external_url": "https://metro-cc.ru",
      "icon_url": "https://cdn.petrushka.ru/icons/metro.png"
    },
    {
      "id": 2,
      "name": "Ашан",
      "delivery_info": "Ближайшая доставка сегодня 18:00–20:00",
      "external_url": "https://www.auchan.ru",
      "icon_url": "https://cdn.petrushka.ru/icons/auchan.png"
    },
    {
      "id": 3,
      "name": "ВкусВилл",
      "delivery_info": "Быстрая доставка от 20 до 60 минут",
      "external_url": "https://www.vkusvill.ru",
      "icon_url": "https://cdn.petrushka.ru/icons/vkusvill.png"
    },
    {
      "id": 4,
      "name": "ВИКТОРИЯ",
      "delivery_info": "Ближайшая доставка сегодня 17:00–19:00",
      "external_url": "https://www.victoria.ru",
      "icon_url": "https://cdn.petrushka.ru/icons/victoria.png"
    }
  ]
}

