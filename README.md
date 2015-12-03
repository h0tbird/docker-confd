# docker-confd

[![Build Status](https://travis-ci.org/h0tbird/docker-confd.svg?branch=master)](https://travis-ci.org/h0tbird/docker-confd)

A containerized confd service:

```
docker run -it --rm \
--name confd \
--net host \
--volume /etc/confd:/etc/confd \
h0tbird/confd \
-node 127.0.0.1:2379 \
-watch
```
