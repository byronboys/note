# GO 命令行
```
1. go get 安装包
-u 更新包和依赖关系，默认情况不更新本地已有包
-v 打印安装包详情
2. go env 查看环境变量
3. go run hello.go 运行
4. go build 构建
5. go help command 查看命令手册
```

## ubuntu install go
```
apt install golang
apt install php7.4 php7.4-cli php7.4-fpm
apt install mysql-server
apt install redis-server
redis-server /etc/redis/redis.conf
```

## /usr/bin /usr/local/bin /usr/local/sbin
```
/usr/bin 系统预装程序
/usr/local/bin 用户安装程序，不需要 root 执行
/usr/local/sbin 用户安装程序，需要 root 执行
```

## 阿里云镜像
```
Windows
打开你的 PowerShell 并执行
$env:GO111MODULE = "on"
$env:GOPROXY="https://mirrors.aliyun.com/goproxy/,direct"

参考链接：https://goproxy.cn/
```