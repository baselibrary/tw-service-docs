## Rubygems源使用帮助


### 地址

https://mirror.thoughtworks.io/repository/rubygems/

### 说明

Rubygems 仓库镜像

### 使用说明

> 警告 操作前请做好相应备份

修改 Rubygems 默认源
```bash
gem sources  #列出默认源
gem sources --remove https://rubygems.org/  #移除默认源
gem sources -a https://mirror.thoughtworks.io/repository/rubygems/  #添加镜像源
```

针对使用 Gemfile 和 Bundle 的项目
```bash
bundle config mirror.https://rubygems.org https://mirror.thoughtworks.io/repository/rubygems/
```

### 参考链接

- 官方主页:	https://rubygems.org/
