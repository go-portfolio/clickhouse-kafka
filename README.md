
## Сборка образа продюсера
Перейдите в папку `producer` с Dockerfile и создайте образ:
```bash
    docker build -t go-kafka-producer .
```    

Запустите продюсер:
```bash
docker run --rm --name go-kafka-producer --network your_network go-kafka-producer
```

## Сборка образа консумера
Перейдите в папку с Dockerfile для консюмера и создайте образ:
```bash
docker build -t go-kafka-consumer .
```

Запустите консюмера:
```bash
docker run --rm --name go-kafka-consumer --network your_network go-kafka-consumer
```