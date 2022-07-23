# 备忘录清单
一个基于gin+gorm开发的练手小项目，通过该项目可初识go web开发该有的姿势。
前端部分源码地址：[bubble_front](https://github.com/starine/bubble_front)。

## 使用指南
### 下载
```bash
git clone https://github.com/Q1mi/bubble.git
```
### 配置MySQL
1. 在你的数据库中执行以下命令，创建本项目所用的数据库：
```sql
CREATE DATABASE bubble DEFAULT CHARSET=utf8mb4;
```
2. 在`bubble/conf/config.ini`文件中按如下提示配置数据库连接信息。

```ini
port = 9000
release = false

[mysql]
user = 你的数据库用户名
password = 你的数据库密码
host = 你的数据库host地址
port = 你的数据库端口
db = bubble
```

### 编译
```bash
go build
```

### 执行

Mac/Unix：
```bash
./bubble conf/config.ini
```
Windows:
```bash
bubble.exe conf/config.ini
```

启动之后，使用浏览器打开`http://127.0.0.1:8080/`即可。

