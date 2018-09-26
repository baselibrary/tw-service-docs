## EPEL源使用帮助


### 地址

https://mirror.thoughtworks.io/repository/epel/

### 说明

EPEL (Extra Packages for Enterprise Linux) 是由 Fedora Special Interest Group 为企业 Linux 创建、维护和管理的一个高质量附加包集合，适用于但不仅限于 Red Hat Enterprise Linux (RHEL), CentOS, Scientific Linux (SL), Oracle Linux (OL)

### 收录版本

官方支持的所有架构

### 使用说明

> 警告 操作前请做好相应备份

执行以下命令：

```bash
sudo yum install -y epel-release
sudo sed -e 's!^mirrorlist=!#mirrorlist=!g' \
         -e 's!^#baseurl=!baseurl=!g' \
         -e 's!//download\.fedoraproject\.org/pub!//mirror.thoughtworks.io/repository!g' \
         -i /etc/yum.repos.d/epel.repo /etc/yum.repos.d/epel-testing.repo
```

### 参考链接

- WIKI:	https://fedoraproject.org/wiki/EPEL
- FAQ:	https://fedoraproject.org/wiki/EPEL/faq
