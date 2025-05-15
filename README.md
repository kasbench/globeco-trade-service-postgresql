# globeco-trade-service-postgresql
PostgreSQL database for the GlobeCo Trade Service.


To build:

```
docker build -t kasbench/globeco-trade-service-postgresql .
```

To run:

```
docker run -d --name globeco-trade-service-postgresql \
  -p 32800:5432 \
  -e POSTGRES_HOST_AUTH_METHOD=trust \
  kasbench/globeco-trade-service-postgresql
```

With network

```
docker run -d --name globeco-trade-service-postgresql \
  -p 32800:5432 \
  -e POSTGRES_HOST_AUTH_METHOD=trust \
  --network my-network \
  kasbench/globeco-trade-service-postgresql
```
