## Maven源使用帮助


### 地址

https://mirror.thoughtworks.io/repository/maven-public/

### 说明

Maven 软件源

### 使用说明

> 警告 操作前请做好相应备份

修改maven根目录下的conf文件夹中的setting.xml文件，内容如下：
```xml
<mirrors>
    <mirror>
      <id>thoughtworks</id>
      <name>Thoughtworks Maven Repo</name>
      <url>https://mirror.thoughtworks.io/repository/maven-public/</url>
      <mirrorOf>central</mirrorOf>        
    </mirror>
  </mirrors>
```

### 参考链接
