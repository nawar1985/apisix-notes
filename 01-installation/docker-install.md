# Docker Installation

## Run APISIX + etcd

```bash
docker network create apisix

docker run -d --name etcd \
  --network apisix \
  quay.io/coreos/etcd:latest
