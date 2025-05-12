# globeco-trade-service-postgresql
PostgreSQL database for the GlobeCo Trade Service.


To build:

```
docker build -t kasbench/globeco-trade-service-posgresql .
```

To run:

```
docker run -d --name globeco-trade-service-postgresql \
  -p 5432:5432 \
  -e POSTGRES_HOST_AUTH_METHOD=trust \
  kasbench/globeco-trade-service-posgresql
```

With network

```
docker run -d --name globeco-order-service-postgresql \
  -p 5432:5432 \
  -e POSTGRES_HOST_AUTH_METHOD=trust \
  --network my-network \
  kasbench/globeco-trade-service-posgresql
```
