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

# Run details service on port 8081
docker run -d --name details -p 8081:9080 details
```

* Test with path `/details/1` and `/health`

## Available Environment Variables
- ENABLE_EXTERNAL_BOOK_SERVICE : ```boolean```
- DO_NOT_ENCRYPT : ```boolean```

## Website

[Opsta (Thailand) Co., Ltd.](https://www.opsta.co.th)