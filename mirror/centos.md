## CentOS 源使用帮助


### 地址

https://mirror.thoughtworks.io/repository/centos/

### 说明

CentOS 软件源

### 收录版本

所有 CentOS 当前支持的版本

### 使用说明

> 警告 操作前请做好相应备份

首先备份 `CentOS-Base.repo`

```bash
mv /etc/yum.repos.d/CentOS-Base.repo /etc/yum.repos.d/CentOS-Base.repo.backup
```

下载对应版本的 `CentOS-Base.repo` , 放入 `/etc/yum.repos.d/`

这是 CentOS 5 的：
```ini
# CentOS-Base.repo
#
# The mirror system uses the connecting IP address of the client and the
# update status of each mirror to pick mirrors that are updated to and
# geographically close to the client.  You should use this for CentOS updates
# unless you are manually picking other mirrors.
#
# If the mirrorlist= does not work for you, as a fall back you can try the
# remarked out baseurl= line instead.
#
#

[base]
name=CentOS-$releasever - Base - mirrors.ustc.edu.cn
baseurl=https://mirror.thoughtworks.io/repository/centos/$releasever/os/$basearch/
#mirrorlist=https://mirrorlist.centos.org/?release=$releasever&arch=$basearch&repo=os
gpgcheck=1
gpgkey=https://mirror.thoughtworks.io/repository/centos/RPM-GPG-KEY-CentOS-5

#released updates
[updates]
name=CentOS-$releasever - Updates - mirrors.ustc.edu.cn
baseurl=https://mirror.thoughtworks.io/repository/centos/$releasever/updates/$basearch/
#mirrorlist=https://mirrorlist.centos.org/?release=$releasever&arch=$basearch&repo=updates
gpgcheck=
gpgkey=https://mirror.thoughtworks.io/repository/centos/RPM-GPG-KEY-CentOS-5

#additional packages that may be useful
[extras]
name=CentOS-$releasever - Extras - mirrors.ustc.edu.cn
baseurl=https://mirror.thoughtworks.io/repository/centos/$releasever/extras/$basearch/
#mirrorlist=https://mirrorlist.centos.org/?release=$releasever&arch=$basearch&repo=extras
gpgcheck=1
gpgkey=https://mirror.thoughtworks.io/repository/centos/RPM-GPG-KEY-CentOS-5

#packages used/produced in the build but not released
[addons]
name=CentOS-$releasever - Addons - mirrors.ustc.edu.cn
baseurl=https://mirror.thoughtworks.io/repository/centos/$releasever/addons/$basearch/
#mirrorlist=https://mirrorlist.centos.org/?release=$releasever&arch=$basearch&repo=addons
gpgcheck=1
gpgkey=https://mirror.centos.org/centos/RPM-GPG-KEY-CentOS-5

#additional packages that extend functionality of existing packages
[centosplus]
name=CentOS-$releasever - Plus - mirrors.ustc.edu.cn
baseurl=https://mirror.thoughtworks.io/repository/centos/$releasever/centosplus/$basearch/
#mirrorlist=https://mirrorlist.centos.org/?release=$releasever&arch=$basearch&repo=centosplus
gpgcheck=1
enabled=0
gpgkey=https://mirror.thoughtworks.io/repository/centos/RPM-GPG-KEY-CentOS-5

#contrib - packages by Centos Users
[contrib]
name=CentOS-$releasever - Contrib - mirrors.ustc.edu.cn
baseurl=https://mirror.thoughtworks.io/repository/centos/$releasever/contrib/$basearch/
#mirrorlist=https://mirrorlist.centos.org/?release=$releasever&arch=$basearch&repo=contrib
gpgcheck=1
enabled=0
gpgkey=https://mirror.thoughtworks.io/repository/centos/RPM-GPG-KEY-CentOS-5
```

这是 CentOS 6 的：
```ini
# CentOS-Base.repo
#
# The mirror system uses the connecting IP address of the client and the
# update status of each mirror to pick mirrors that are updated to and
# geographically close to the client.  You should use this for CentOS updates
# unless you are manually picking other mirrors.
#
# If the mirrorlist= does not work for you, as a fall back you can try the
# remarked out baseurl= line instead.
#
#

[base]
name=CentOS-$releasever - Base - mirrors.ustc.edu.cn
baseurl=https://mirror.thoughtworks.io/repository/centos/$releasever/os/$basearch/
#mirrorlist=https://mirrorlist.centos.org/?release=$releasever&arch=$basearch&repo=os
gpgcheck=1
gpgkey=https://mirror.thoughtworks.io/repository/centos/RPM-GPG-KEY-CentOS-6

#released updates
[updates]
name=CentOS-$releasever - Updates - mirrors.ustc.edu.cn
baseurl=https://mirror.thoughtworks.io/repository/centos/$releasever/updates/$basearch/
#mirrorlist=https://mirrorlist.centos.org/?release=$releasever&arch=$basearch&repo=updates
gpgcheck=1
gpgkey=https://mirror.thoughtworks.io/repository/centos/RPM-GPG-KEY-CentOS-6

#additional packages that may be useful
[extras]
name=CentOS-$releasever - Extras - mirrors.ustc.edu.cn
baseurl=https://mirror.thoughtworks.io/repository/centos/$releasever/extras/$basearch/
#mirrorlist=https://mirrorlist.centos.org/?release=$releasever&arch=$basearch&repo=extras
gpgcheck=1
gpgkey=https://mirror.thoughtworks.io/repository/centos/RPM-GPG-KEY-CentOS-6

#additional packages that extend functionality of existing packages
[centosplus]
name=CentOS-$releasever - Plus - mirrors.ustc.edu.cn
baseurl=https://mirror.thoughtworks.io/repository/centos/$releasever/centosplus/$basearch/
#mirrorlist=https://mirrorlist.centos.org/?release=$releasever&arch=$basearch&repo=centosplus
gpgcheck=1
enabled=0
gpgkey=https://mirror.thoughtworks.io/repository/centos/RPM-GPG-KEY-CentOS-6

#contrib - packages by Centos Users
[contrib]
name=CentOS-$releasever - Contrib - mirrors.ustc.edu.cn
baseurl=https://mirror.thoughtworks.io/repository/centos/$releasever/contrib/$basearch/
#mirrorlist=https://mirrorlist.centos.org/?release=$releasever&arch=$basearch&repo=contrib
gpgcheck=1
enabled=0
gpgkey=https://mirror.thoughtworks.io/repository/centos/RPM-GPG-KEY-CentOS-6
```

这是 CentOS 7 的：
```ini
# CentOS-Base.repo
#
# The mirror system uses the connecting IP address of the client and the
# update status of each mirror to pick mirrors that are updated to and
# geographically close to the client.  You should use this for CentOS updates
# unless you are manually picking other mirrors.
#
# If the mirrorlist= does not work for you, as a fall back you can try the
# remarked out baseurl= line instead.
#
#

[base]
name=CentOS-$releasever - Base
#mirrorlist=https://mirrorlist.centos.org/?release=$releasever&arch=$basearch&repo=os
baseurl=https://mirror.thoughtworks.io/repository/centos/$releasever/os/$basearch/
gpgcheck=1
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7

#released updates
[updates]
name=CentOS-$releasever - Updates
# mirrorlist=https://mirrorlist.centos.org/?release=$releasever&arch=$basearch&repo=updates
baseurl=https://mirror.thoughtworks.io/repository/centos/$releasever/updates/$basearch/
gpgcheck=1
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7

#additional packages that may be useful
[extras]
name=CentOS-$releasever - Extras
# mirrorlist=https://mirrorlist.centos.org/?release=$releasever&arch=$basearch&repo=extras
baseurl=https://mirror.thoughtworks.io/repository/centos/$releasever/extras/$basearch/
gpgcheck=1
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7

#additional packages that extend functionality of existing packages
[centosplus]
name=CentOS-$releasever - Plus
# mirrorlist=https://mirrorlist.centos.org/?release=$releasever&arch=$basearch&repo=centosplus
baseurl=https://mirror.thoughtworks.io/repository/centos/$releasever/centosplus/$basearch/
gpgcheck=1
enabled=0
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7
```

运行 `sudo yum makecache` 生成缓存。

### 参考链接

- 官方主页:	https://www.centos.org/
- 邮件列表:	https://www.centos.org/modules/tinycontent/index.php?id=16
- 论坛:	https://www.centos.org/modules/newbb/
- 文档:	https://www.centos.org/docs/
- Wiki:	https://wiki.centos.org/
- 镜像列表:	https://www.centos.org/modules/tinycontent/index.php?id=32
