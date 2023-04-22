# Использование

### Запуск:
1. ```docker build -t stocks_products .```
2. ```docker run -d -p 1010:1010 stocks_products```
3. [http://127.0.0.1:1010/api/v1/](http://127.0.0.1:1010/api/v1/)
### Проверка HTTP-запросов:
- **GET**  
Спиоск всех продуктов ```curl localhost:1010/api/v1/products/```  
Список всех складов ```curl localhost:1010/api/v1/stocks/```

[//]: # ()
[//]: # (- **POST**  )

[//]: # (Создание продукта ```curl -X POST localhost:1010/api/v1/products/ -H 'Content-Type: application/json' -d '{"title": "Баклажан", "description": "Лучшие помидоры на рынке"}'```  )

[//]: # (Создание склада ```curl -X POST localhost:1010/api/v1/stocks/ -H 'Content-Type: application/json' -d '[{"product": 2, "quantity": 250, "price": 120.50}, {"product": 3, "quantity": 100, "price": 180}]'``` )
