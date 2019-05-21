# musql
mysql一些基本信息

1 ubuntu安装mysql
* 服务端：sudo apt-get install mysql-server
* 客户端：sudo apt-get install mysql-client
2 windows
* 下载安装包 mysql-installerxxx.5.7.xxx.msi
3 启动和链接MySQL服务
* 服务端启动
	sudo /etc/init.d/mysql start|status|stop|restart
	sudo service mysql start|status|stop|restart
* 客户端链接
	* mysql -hIP地址 -u用户名 -p密码  (这里的root是mysql的root，不是linux的root)
	mysql -h127.0.0.1 -uroot -p123456   
	mysql -hlocalhost -uroot -p123456 
	mysql -uroot -p123456 本地登录可以省略-h选项
  
4 安装pip
	sudo apt-get install python3-pip
5 在线安装第三方模块
	sudo pip3 install pymysql
6 离线安装第三方模块
	下载安装包 .tar.gz
	解压: tar -zvf pymysql.tar.gz
	cd到解压文件夹，找setup.py　README
	sudo python3 setup.py install
