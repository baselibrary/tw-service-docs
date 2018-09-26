## Ubuntu 源使用帮助


### 地址

https://mirror.thoughtworks.io/repository/ubuntu/

### 说明

Ubuntu 软件源

### 收录版本

所有 Ubuntu 当前支持的版本

### 使用说明

> 警告 操作前请做好相应备份

#### 图形界面配置

新手推荐使用图形界面配置： 系统设置 -> 软件和更新 选择下载服务器 -> "mirror.thoughtworks.io/repository/ubuntu"

#### 手动更改配置

用你熟悉的编辑器打开：

/etc/apt/sources.list

替换默认的 `https://archive.ubuntu.com/` 为 `https://mirror.thoughtworks.io/repository/ubuntu/`

以Ubuntu 14.04.5 LTS为例，最后的效果如下：
```vim
deb https://mirror.thoughtworks.io/repository/ubuntu/ trusty main restricted universe multiverse
deb-src https://mirror.thoughtworks.io/repository/ubuntu/ trusty main restricted universe multiverse
deb https://mirror.thoughtworks.io/repository/ubuntu/ trusty-security main restricted universe multiverse
deb-src https://mirror.thoughtworks.io/repository/ubuntu/ trusty-security main restricted universe multiverse

deb https://mirror.thoughtworks.io/repository/ubuntu/ trusty-updates main restricted universe multiverse
deb-src https://mirror.thoughtworks.io/repository/ubuntu/ trusty-updates main restricted universe multiverse

deb https://mirror.thoughtworks.io/repository/ubuntu/ trusty-backports main restricted universe multiverse
deb-src https://mirror.thoughtworks.io/repository/ubuntu/ trusty-backports main restricted universe multiverse

## Not recommended
# deb https://mirror.thoughtworks.io/repository/ubuntu/ trusty-proposed main restricted universe multiverse
# deb-src https://mirror.thoughtworks.io/repository/ubuntu/ trusty-proposed main restricted universe multiverse
```

ubuntu 16.04 配置如下
```vim
deb https://mirror.thoughtworks.io/repository/ubuntu/ xenial main
deb-src https://mirror.thoughtworks.io/repository/ubuntu/ xenial main

deb https://mirror.thoughtworks.io/repository/ubuntu/ xenial-updates main
deb-src https://mirror.thoughtworks.io/repository/ubuntu/ xenial-updates main

deb https://mirror.thoughtworks.io/repository/ubuntu/ xenial universe
deb-src https://mirror.thoughtworks.io/repository/ubuntu/ xenial universe
deb https://mirror.thoughtworks.io/repository/ubuntu/ xenial-updates universe
deb-src https://mirror.thoughtworks.io/repository/ubuntu/ xenial-updates universe

deb https://mirror.thoughtworks.io/repository/ubuntu/ xenial-security main
deb-src https://mirror.thoughtworks.io/repository/ubuntu/ xenial-security main
deb https://mirror.thoughtworks.io/repository/ubuntu/ xenial-security universe
deb-src https://mirror.thoughtworks.io/repository/ubuntu/ xenial-security universe
```

ubuntu 18.04(bionic) 配置如下
```vim
deb https://mirror.thoughtworks.io/repository/ubuntu/ bionic main restricted universe multiverse
deb-src https://mirror.thoughtworks.io/repository/ubuntu/ bionic main restricted universe multiverse

deb https://mirror.thoughtworks.io/repository/ubuntu/ bionic-security main restricted universe multiverse
deb-src https://mirror.thoughtworks.io/repository/ubuntu/ bionic-security main restricted universe multiverse

deb https://mirror.thoughtworks.io/repository/ubuntu/ bionic-updates main restricted universe multiverse
deb-src https://mirror.thoughtworks.io/repository/ubuntu/ bionic-updates main restricted universe multiverse

deb https://mirror.thoughtworks.io/repository/ubuntu/ bionic-proposed main restricted universe multiverse
deb-src https://mirror.thoughtworks.io/repository/ubuntu/ bionic-proposed main restricted universe multiverse

deb https://mirror.thoughtworks.io/repository/ubuntu/ bionic-backports main restricted universe multiverse
deb-src https://mirror.thoughtworks.io/repository/ubuntu/ bionic-backports main restricted universe multiverse
```

### 参考链接

- 官方主页: https://www.ubuntu.com/
- 邮件列表: https://www.ubuntu.com/support/community/mailinglists
- 论坛: https://ubuntuforums.org/
- 中文论坛: https://forum.ubuntu.org.cn/
- Wiki: https://wiki.ubuntu.com/
- 帮助: https://help.ubuntu.com/
