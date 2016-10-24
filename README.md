CentOS Images
===============

Docker images build from centos7


Preparation
-------------

```docker pull centos:7.2.1511``` or ```docker pull hub.c.163.com/library/centos:7.2.1511``` (from 163 mirror)


Building
----------

Build each image

```
https://github.com/seandou/centos-images.git

# cd <image path>

docker build -t <your-tag> .
```


References
------------

- [The official build of CentOS](https://hub.docker.com/_/centos/)

### China mirrors

- [阿里云镜像仓库](https://cr.console.aliyun.com/#/imageList)
- [网易蜂巢 DH 镜像](https://c.163.com/hub#/m/library/)
