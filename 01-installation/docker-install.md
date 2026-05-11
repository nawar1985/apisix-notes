# Docker Installation

## Run APISIX + etcd

```bash
docker network create apisix

docker run -d --name etcd \
  --network apisix \
  quay.io/coreos/etcd:latest

docker run -d --name apisix \
  --network apisix \
  -p 9080:9080 \
  -p 9180:9180 \
  apache/apisix
