# confd

[![Build Status](https://travis-ci.org/katosys/confd.svg?branch=master)](https://travis-ci.org/katosys/confd)

A containerized confd service:

```
docker run -it --rm \
--name confd \
--net host \
--volume /etc:/host/etc \
--volume /run:/host/run \
--volume /etc/confd:/etc/confd \
quay.io/kato/confd:v0.13.0-1 \
-node http://127.0.0.1:2379 \
-watch
```
