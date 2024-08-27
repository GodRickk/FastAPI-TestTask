# Приложение для учета товаров и их категорий

## Локальный запуск

1. Установите зависимости с помощью Poetry:
`poetry install`

2. Запустите приложение: 
`poetry run uvicorn main:app --reload`

3. API будет доступно по адресу http://127.0.0.1:8000/docs#/ (удобная версия для теста запросов)


## Запуск с использованием Docker

1. Соберите и запустите контейнер
   ``` bash
   docker-compose up --build
   ```
API будет доступно по адресу http://127.0.0.1:8000/docs#/ (удобная версия для теста запросов)


## Запуск тестов

Запуск тестов осуществляется командой:
`poetry run pytest tests/`


## Использование API
по адресу http://127.0.0.1:8000/docs#/ располагается удобный интерфейс для отправки всех типов запросов GET, POST, PATCH, DELETE

Реализованные доступные функции:
### POST
   #### product
   - create_product - создание продукта без категории (по умолчанию None)
   
   - create_product_with_category - создание продукта с указанием существующей категории

   #### category
   - create_category - создание категории с указанием имени
### GET
   #### product
   

   
