
# Сборка образа продьюсера
Перейдите в папку `producer` с Dockerfile и создайте образ:
```bash
    docker build -t go-kafka-producer .
```    

Запустите продюсер:
```bash
docker run --rm --name go-kafka-producer --network your_network go-kafka-producer
```