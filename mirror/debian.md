## Debian 源使用帮助


### 地址

https://mirror.thoughtworks.io/repository/debian/

### 说明

Debian 软件源

### 收录版本

所有 Debian 当前支持的版本

### 使用说明

> 警告 操作前请做好相应备份

一般情况下，将 `/etc/apt/sources.list` 文件中 Debian 默认的源地址 `https://deb.debian.org/debian` 替换为 `https://mirror.thoughtworks.io/repository/debian` 即可。

可以使用如下命令：

```bash
sudo sed -i 's|deb.debian.org/debian|mirror.thoughtworks.io/repository/debian|g' /etc/apt/sources.list
```

当然也可以直接编辑 `/etc/apt/sources.list` 文件（需要使用 sudo）。以下是 Debian Stable 参考配置内容：
```vim
deb https://mirror.thoughtworks.io/repository/debian stable main contrib non-free
# deb-src https://mirror.thoughtworks.io/repository/debian stable main contrib non-free
deb https://mirror.thoughtworks.io/repository/debian stable-updates main contrib non-free
# deb-src https://mirror.thoughtworks.io/repository/debian stable-updates main contrib non-free

# deb https://mirror.thoughtworks.io/repository/debian stable-proposed-updates main contrib non-free
# deb-src https://mirror.thoughtworks.io/repository/debian stable-proposed-updates main contrib non-free
```

同时你也可能需要更改 Debian Security 源，请参考 Debian Security 源使用帮助

更改完 sources.list 文件后请运行 `sudo apt-get update` 更新索引以生效。

### 参考链接

- 官方主页:	https://www.debian.org/
- 邮件列表:	https://www.debian.org/MailingLists/
- Wiki:	https://wiki.debian.org/
- 文档:	https://www.debian.org/doc/
- 镜像列表:	https://www.debian.org/mirror/list
