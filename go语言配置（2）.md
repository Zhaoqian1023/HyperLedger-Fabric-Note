### go语言配置（2）
##### 版本要求
```
 要求：go version 1.10.x以上
 本次实验使用版本1.10.1
```
##### 步骤
1、下载go语言版本包
```
$ wget https://storage.googleapis.com/golang/go1.10.1.linux-amd64.tar.gz^C
```
2、解包到/usr/local
```
$ sudo tar -xzf go1.10.1.linux-amd64.tar.gz -C /usr/local
```
3、新建go工作文件夹
```
$ cd ~
$ mkdir go
```
4、添加环境变量
```
$ vim ~/.profile
文件末尾新增一下内容：
export PATH=$PATH:/usr/local/go/bin
export GOROOT=/usr/local/go
export GOPATH=$HOME/go
export PATH=$PATH:$HOME/go/bin
```
5、使配置文件生效
```
$ source ~/.profile
```
6、检验安装效果
```
$ go version
```
