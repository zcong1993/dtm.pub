# 直接部署

## 获取二进制文件

dtm暂不支持apt/yum/brew等方式直接安装，您需要通过go环境，编译出相关的二进制文件，因此不是很推荐这种方式部署。

## 编译

您需要有go 1.15以上的环境，通过下面命令编译出二进制文件
```
go build -o dtm app/main.go
```

## 配置

您可以设置相关的环境变量(参见[部署基础](./base))，也可以在工作目录下，参考[配置样板文件](https://github.com/yedf/dtm/blob/main/conf.sample.yml)创建conf.yml文件

## 启动

dtm会监听8080端口

```
./dtm dtmsvr
```