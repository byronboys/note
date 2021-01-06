### HK 测试环境

```
#ssh
8.210.4.64
root / rFhY=9x4T@p6WS-d

HKDEMO数据库：
host：a4l-polardb-testdb.mysql.polardb.rds.aliyuncs.com
用户：polardbadmin
密码：Glb7yv*UrP
数据库：all4learn-hkdemo

hkdemo site is now password protected. 
Url: https://hkdemo.all4learn.com
Userid: demo01
Password: alllearn
```

### 开发环境： 8.129.108.170

```
root / Q89mB^Fhas^Ym_8r
mysql：8.129.108.170:3306
用户： root  密码：Dev!@#$%^
用户： DevDB  密码：Dev!@#$%^

DB_DSN           = mysql:host=a4l-polardb-testdb.mysql.polardb.rds.aliyuncs.com;port=3306;dbname=all4learn
DB_USERNAME      = polardbadmin
DB_PASSWORD      = Glb7yv*UrP
```

### 测试服务器：47.115.174.184

```
root / a/9At7BzWNg6mk<8
```


### [laravel大中型设计模式](https://blog.csdn.net/qq_24935119/article/details/89656569)

```
#Repository 数据库相关操作，依赖Model

Model 表相关属性、关联关系 ORM 类，不参与实际业务逻辑
Service 业务逻辑处理层，依赖Repository
Controller 依赖Service



CURD
C => Create
U => update
R => Read
D => Delete

Solid

S => 单一原则 解耦
O => 开闭原则 容易拓展
L => 里氏替换原则 解耦、拓展
I => 接口隔离原则 专注单一
D => 依赖倒置原则 解耦、方便测试
```

### FAQ
```
1. Laravel框架
    - Composer包丰富，下载快
    - 版本更新很快，1年发1个大版本，几个月发一个小版本
    - 使用率高，GitHub PHP框架占有率47%
    - 设计模式很新，分层很好，代码很优雅
    - 开发、部署、线上、架构
    - 招人

2. 发布系统
3. 监控系统
4. 后台系统。（配置、数据统计）
```