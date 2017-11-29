# RabbitMQ Plugins Box

Storing RabbitMQ 3.6.x plugins by Alpine.

[![](https://img.shields.io/badge/Github-thxcode/rabbitmq--plugins--box-orange.svg)](https://github.com/thxcode/rabbitmq-plugins-box)&nbsp;[![](https://img.shields.io/badge/Docker_Hub-maiwj/rabbitmq--plugins--box-orange.svg)](https://hub.docker.com/r/maiwj/rabbitmq-plugins-box)&nbsp;[![](https://img.shields.io/docker/build/maiwj/rabbitmq-plugins-box.svg)](https://hub.docker.com/r/maiwj/rabbitmq-plugins-box)&nbsp;[![](https://img.shields.io/docker/pulls/maiwj/rabbitmq-plugins-box.svg)](https://store.docker.com/community/images/maiwj/rabbitmq-plugins-box)&nbsp;[![](https://img.shields.io/github/license/thxcode/rabbitmq-plugins-box.svg)](https://github.com/thxcode/rabbitmq-plugins-box)

[![](https://images.microbadger.com/badges/image/maiwj/rabbitmq-plugins-box.svg)](https://microbadger.com/images/maiwj/rabbitmq-plugins-box)&nbsp;[![](https://images.microbadger.com/badges/version/maiwj/rabbitmq-plugins-box.svg)](http://microbadger.com/images/maiwj/rabbitmq-plugins-box)&nbsp;[![](https://images.microbadger.com/badges/commit/maiwj/rabbitmq-plugins-box.svg)](http://microbadger.com/images/maiwj/rabbitmq-plugins-box.svg)

## References

### Plugin List

- [RabbitMQ Autocluster 0.10.0](https://github.com/rabbitmq/rabbitmq-autocluster/releases/tag/0.10.0)

## How to use this image

### Start an instance

To start a container, use the following:

``` bash
$ docker run -it --name test-rpb maiwj/rabbitmq-plugins-box
```

### Get list from Kubernetes Pod

``` bash
$ kubectl run -it --image maiwj/rabbitmq-plugins-box:latest test bash

/# ls -al /plugins
total 176
drwxr-xr-x    1 root     root          4096 Nov 29 02:32 .
drwxr-xr-x    1 root     root          4096 Nov 29 02:32 ..
-rw-------    1 root     root        104967 Oct 19 19:15 autocluster-0.10.0.ez
-rw-------    1 root     root         65012 Oct 19 19:15 rabbitmq_aws-0.10.0.ez

```

## License

- RabbitMQ Autocluster is released under the [BSD-3-Clause License](https://github.com/rabbitmq/rabbitmq-autocluster/blob/master/LICENSE)
- This image is released under the [MIT License](LICENSE)
