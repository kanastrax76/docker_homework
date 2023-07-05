Создание образа


docker build ./ --tag stockproducts:1.0


Запуск контейнера


docker run -d --name crud_stockproducts -p 8000:8000 stockproducts:1.0
