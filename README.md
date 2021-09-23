# ClamAV via HTTP server

## Getting started

### Run

```bash
git submodule init
docker-compose up --build -d
```

## Tests

```bash
docker-compose up --build -d
curl -F "name=blabla" -F "file=@./tests/samples/eicar.txt" localhost:8080/scanReply --output -
```
