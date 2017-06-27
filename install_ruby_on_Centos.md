请参考如下 ：
http://blog.csdn.net/shuai825644975/article/details/53446621
=====================================================================================

1. edis3.0以上支持集群，自带集群管理工具redis-trib.rb；在搭建集群前，安装ruby环境

ruby安装包下载：
http://download.csdn.net/detail/shuai825644975/9700933
  
安装开发工具:
1、命令：yum groupinstall "Development tools"

清理已安装过的
2、命令：yum erase ruby ruby-libs ruby-mode ruby-rdoc ruby-irb ruby-ri ruby-docs

安装依赖
3、命令：yum -y install zlib-devel curl-devel openssl-devel httpd-devel apr-devel apr-util-devel mysql-devel

4、安装ruby

刚开始用命令yum install ruby安装，但是是2.0以下的版本。我把它卸载了，重新下的2.0以上的包安装

把安装包上传到指定目录，并解压

命令：tar zxvf ruby-2.3.0.tar.gz；解压后，进入ruby-2.3.0目录下，依次执行下面命令

命令：./configure

命令：make

命令：make install



5、查看ruby信息

命令：ruby -v



6、要支持redis的通信，需要下载redis相关包

命令：gem install redis

7.  显示gem下载的所有包：
gem list
