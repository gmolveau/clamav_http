# ClamAV via HTTP server

- based on :
    - https://github.com/solita/clamav-rest
    - https://github.com/mko-x/docker-clamav
- inspirations :
    - https://blog.theodo.com/2017/11/implement-antivirus-api-10-min/
    - https://dev.solita.fi/2015/06/02/rest-virusscan.html

## Getting started

### Run

```bash
git submodule update
docker-compose up --build -d
```

## Tests

```bash
docker-compose up --build -d
curl -F "name=blabla" -F "file=@./tests/samples/eicar.txt" localhost:8080/scanReply --output -
```
