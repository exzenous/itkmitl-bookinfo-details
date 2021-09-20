# Bookinfo Details Service

**Details Service** has been *developed* on Ruby

## License

MIT License

## Prerequisite

- Ruby 2.7

## How to run

```bash
ruby details.rb 9080
```

## How to run with Docker

```bash
# Build Docker Image for details service
docker build -t details .

# # Run MongoDB with initial data in database
# docker run -d --name mongodb -p 27017:27017 \
#   -v $(pwd)/databases:/docker-entrypoint-initdb.d bitnami/mongodb:5.0.2-debian-10-r2

# Run details service on port 8081
docker run -d --name details -p 8081:9080 details
# docker run -d --name details -p 8081:9080 --link mongodb:mongodb \
#   -e SERVICE_VERSION=v2 -e 'MONGO_DB_URL=mongodb://mongodb:27017/ratings' ratings
```

* Test with path `/details/1` and `/health`

## Website

[Opsta (Thailand) Co., Ltd.](https://www.opsta.co.th)