## PyPi源使用帮助


### 地址

https://mirror.thoughtworks.io/repository/pypi/

### 说明

PyPi(pip) 软件源

### 使用说明

> 警告 操作前请做好相应备份

在文件 `~/.pip/pip.conf` 中添加或修改:
```ini
[global]
index-url = https://mirror.thoughtworks.io/repository/pypi/simple/

[install]
trusted-host=mirror.thoughtworks.io
```

### 参考链接

- PyPI Official Mirrors: https://pypi.python.org/mirrors
- PEP-381 Mirroring Protocol: https://www.python.org/dev/peps/pep-0381/
- bandersnatch: https://pypi.python.org/pypi/bandersnatch
