# 1. 安装 golang
1. 下载源码
```sh
$ cd /usr/local/src/
$ wget https://storage.googleapis.com/golang/go1.8.3.linux-amd64.tar.gz
```
2. 解压源码
```sh
$ tar -C /usr/local -xzf go1.8.3.linux-amd64.tar.gz
```
3. 配置环境变量
```sh
$ vim /etc/profile
```
在 export PATH USER LOGNAME MAIL HOSTNAME HISTSIZE HISTCONTROL 一行的上面添加如下内容:
```v
# set for golang
export GO_HOME=/usr/local/go
export PATH=$GO_HOME/bin:$PATH
```
4. 配置生效
```sh
$ source /etc/profile
```
5. 验证是否安装配置成功
```sh
$ go version
```

# 2. 安装 node.js
1. 下载源码
```sh
$ cd /usr/local/src/
$ wget http://nodejs.org/dist/v7.10.0/node-v7.10.0.tar.gz
```
2. 解压源码
```sh
$ tar zxvf node-v7.10.0.tar.gz
```
3. 编译安装
```sh
$ cd node-v7.10.0
$ ./configure --prefix=/usr/local/node/7.10.0
$ make && make install
```
4. 配置环境变量
```sh
$ vim /etc/profile
```
在 export PATH USER LOGNAME MAIL HOSTNAME HISTSIZE HISTCONTROL 一行的上面添加如下内容:
```v
# set for nodejs
export NODE_HOME=/usr/local/node/7.10.0
export PATH=$NODE_HOME/bin:$PATH
```
5. 配置生效
```sh
$ source /etc/profile
```
6. 验证是否安装配置成功
```sh
$ node -v
```
# 3. 安装 redis
1. 下载源码
```sh
$ cd /usr/local/src/
$ wget http://download.redis.io/releases/redis-3.2.9.tar.gz
```
2. 解压源码
```sh
$ tar zxvf redis-2.8.17.tar.gz
```
3. 编译安装
```sh
$ cd redis-2.8.17
$ make
```
# 4. 安装 postgresql
1. 安装依赖项
```sh
$ yum install -y gcc gcc-c++ make automake 
$ wget http://www.cmake.org/files/v3.8/cmake-3.8.0.tar.gz
$ tar -zxvf cmake-3.8.0.tar.gz
$ cd cmake-3.8.0.tar.gz
$ ./bootstrap
$ yum install readline-devel
```
2. 连接
```
$ pgcli postgres://postgres:@localhost:5432/test
```
