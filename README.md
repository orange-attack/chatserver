# Linux下基于muduo的C++集群聊天服务器
### Introduction
本项目为C++11编写的IM聊天服务器，其特点为：
- 使用 muduo 网络库提供底层的网络I/O；
- 使用 mysql 数据库存放好友、群组等信息；
- 使用 nginx 拓展服务器集群，提高服务器的并发量；
- 基于 redis 的发布-订阅设计消息队列，用于跨服务器的客户端通信；

### Envoirment
OS：Ubuntu 20.04.6
Complier: g++ 9.4.0
C++ 11
MySQL 8.0.34
Nginx 1.21.2
Redis
本项目需要配置的环境较为复杂，请查看
[项目环境配置教程](docs/项目环境配置教程.md)


### Build
./autobuild.sh

### Run
./bin/ChatServer 127.0.0.1 6000

./bin/ChatClient 127.0.0.1 8000

