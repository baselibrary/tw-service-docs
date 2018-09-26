## Docker HUB 源使用帮助


### 地址

https://mirror.thoughtworks.io

### 说明

dockerhub、gcr.io、quay.io 镜像缓存

### 收录版本

所有 dockerhub、gcr.io、quay.io 镜像

### 使用说明

**Linux**

对于使用 upstart 的系统（Ubuntu 14.04、Debian 7 Wheezy），在配置文件 ``/etc/default/docker` 中的 DOCKER_OPTS 中配置Hub地址：
```
DOCKER_OPTS="--registry-mirror=https://mirror.thoughtworks.io"
```
重新启动服务:
```bash
sudo service docker restart
```

对于使用 systemd 的系统（Ubuntu 16.04+、Debian 8+、CentOS 7）， 在配置文件 `/etc/docker/daemon.json` 中加入：
```json
{
  "registry-mirrors": ["https://mirror.thoughtworks.io"]
}
```
重新启动 dockerd：
```bash
sudo systemctl restart docker
```

**MacOS**

* 打开 “Docker.app”
* 进入偏好设置页面(快捷键 ⌘, )
* 打开 “Advanced” 选项卡
* 在 “Registry mirrors” 中添加 `https://mirror.thoughtworks.io`
* 点击下方的 “Restart” 按钮

**Windows**

在系统右下角托盘 Docker 图标内右键菜单选择 `Settings` ，打开配置窗口后左侧导航菜单选择 `Daemon` 。在 `Registry mirrors` 一栏中填写地址 `https://mirror.thoughtworks.io` ，之后点击 `Apply` 保存后 Docker 就会重启并应用配置的镜像地址了。


### 参考链接

- Docker 主页:	https://www.docker.com
- Docker Hub:	https://hub.docker.com
