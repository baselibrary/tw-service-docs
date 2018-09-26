## Docker CE 源使用帮助


### 地址

https://mirror.thoughtworks.io/repository/docker-ce/

### 说明

Docker CE 仓库镜像

### 收录版本

所有 Docker CE 官方支持的版本

### 使用说明

> 警告 操作前请做好相应备份

安装 Docker CE，请按照 [官方安装文档](https://docs.docker.com/engine/installation/)，选择你对应的系统。
```
以 Ubuntu 为例，参考官方Ubuntu安装Docker CE手册(https://docs.docker.com/engine/installation/linux/docker-ce/ubuntu/>) 进行安装。
```

在阅读官方安装手册时，只要把 ``download.docker.com`` 地址换成 ``mirror.thoughtworks.io/repository/docker-ce`` 即可。

[CentOS](https://docs.docker.com/engine/installation/linux/docker-ce/centos/)、
[Fedora](https://docs.docker.com/engine/installation/linux/docker-ce/fedora/)等用户在下载 :file:`docker-ce.repo` 文件后，
还需要将该文件中的 ``download.docker.com`` 地址换成 ``mirror.thoughtworks.io/repository/docker-ce``。

### 参考链接

- Docker 官网: https://www.docker.com/
- Docker Store: https://store.docker.com/
- Docker Hub: https://hub.docker.com/
