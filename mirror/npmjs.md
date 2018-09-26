## PyPi源使用帮助


### 地址

https://mirror.thoughtworks.io/repository/npmjs/

### 说明

NpmJS 软件源

### 使用说明

> 警告 操作前请做好相应备份

临时使用
```bash
npm --registry https://mirror.thoughtworks.io/repository/npmjs install express
```

持久使用
```bash
npm config set registry https://mirror.thoughtworks.io/repository/npmjs

// 配置后可通过下面方式来验证是否成功
npm config get registry
// 或
npm info express
```

通过cnpm使用
```bash
npm install -g cnpm --registry=https://mirror.thoughtworks.io/repository/npmjs

// 使用
cnpm install express
```

### 参考链接
