# 快传<img align="right" width="60" src="https://raw.githubusercontent.com/NXY666/SwiftShare/master/resources/favicon.ico">

## 功能特性
* **传递文本**。零散文本无需保存为文件，可直接传递。
* **传输文件**。支持多文件传输，下载前可指定需要下载的文件。
* **持久共享**。支持设置一个常驻的共享目录，只需将文件放入该目录，即可通过快传传输。每次启动时会生成一个随机的提取码用于下载共享目录中的文件。
* **在线播放**。支持使用提取码在线播放视频，无需下载。
* **深色模式**。当系统处于深色模式时，快传也会自动切换到深色模式。
* **自定义配置**。支持自定义端口、提取码长度、过期时间等多项配置。

## 使用方法
### 安装
```shell
npm install -g swift-share
```

### 配置
```shell
swift-share -config
```

### 启动
```shell
swift-share
```

### 停止
```shell
^C
```

## 注意事项
* 快传未设计任何保护机制，不建议在公网环境下使用。
* 关闭快传后，已上传的文件将**自动删除**，共享文件夹中的文件不受影响。如果出现异常退出，在下次启动时会自动清理未删除的文件。