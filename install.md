# 系统安装
## 必要更新和设置
### 路径换为英文
export LANG=en_US  
xdg-user-dirs-gtk-update  
echo 选 update  
export LANG=zh_CN.UTF-8  
xdg-user-dirs-gtk-update  
echo 选“不要再提醒”和“保持原来的名称”  
* [参考](https://blog.csdn.net/ly890700/article/details/52269254)

## Emacs相关
sudo apt intall emacs  

git clone https://github.com/syl20bnr/spacemacs ~/.emacs.d  
* [spacemacs](http://spacemacs.org/)

## JDK 8
sudo apt-get install openjdk-8-jdk  

## configured directory for incoming file does not exist
You can get the path with  

gsettings get org.blueman.transfer shared-path  

and change it with (for instance)  

gsettings set org.blueman.transfer shared-path '/home/toto'  

* [参考](https://askubuntu.com/questions/837977/configured-directory-for-incoming-file-does-not-exist/901111)


## 安装apache2
sudo apt install apache2  
//测试是否安装成功  
浏览器地址栏输入“localhost”  
//安装最新版php命令  
sudo apt install php  
//配置apache2与php命令  
sudo apt-get install libapache2-mod-php  
//重启apache2命令  
sudo /etc/init.d/apache2 restart  
//测试php，借用W3School上的首个程序  

``` 
 <!DOCTYPE html>
 <html>
 <body>

 <?php
  echo "我的第一段 PHP 脚本！";
 ?>

 </body>
 </html>
```

保存成test.php，复制进/var/www/html目录下  
浏览器地址栏输入localhost/test.php  

## apache2 更改根目录方法

vim /etc/apache2/apache2.conf，把文件里面的/var/www改成你的目标地址。  
vim /etc/apache2/sites-enabled/000-default.conf，把文件里面的/var/www改成你的目标地址。  
service apache2 restart
