<h1 align="center">《Apache安装与使用》1.0</h1>

# xampp下载
####地址：https://www.apachefriends.org/zh_cn/download.html

#Apache搭建站点

- 安装
	- 一路下一步到底
- 基本配置
	- D:\xampp\apache\conf\extra\httpd-vhosts.conf

		   	<VirtualHost *:80>
				DocumentRoot "E:\shop-pc"
				ServerName www.test.shop.com
			</VirtualHost>

	- D:\xampp\apache\conf\httpd.conf

		   	<Directory "D:/xampp/cgi-bin">
    			AllowOverride All
    			Options None
    			Require all granted
			</Directory>

	- C:\Windows\System32\drivers\etc\hosts

		   	127.0.0.1       www.test.shop.com

- 常见的错误（后续慢慢补充）

    - 1 xampp 出现403 无法访问问题（已解决）

    		https://www.cnblogs.com/dubin382460/p/6476347.html