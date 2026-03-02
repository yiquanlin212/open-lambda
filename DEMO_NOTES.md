# OpenLambda Demo (Codespaces)

## Commands (copy & run)
```bash
make ol imgs/ol-min

sudo ./ol worker init -p myworker -i ol-min
sudo ./ol worker up -p myworker

curl -s http://localhost:5000/status

sudo ./ol admin install -n hello -p myworker examples/hello
curl -s -X POST http://localhost:5000/run/hello -d '{}'
