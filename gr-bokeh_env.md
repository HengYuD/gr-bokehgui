## 实验环境

ubuntu16.04
[gnuradio v3.7.13.5(最新版)](https://www.gnuradio.org/releases/gnuradio/)

[gnuradio安装参考]([https://hengyud.cn/Gnuradio-UHD-OpenBTS-%E8%BD%AF%E4%BB%B6%E6%97%A0%E7%BA%BF%E7%94%B5%E5%B9%B3%E5%8F%B0%E6%90%AD%E5%BB%BA/#more](https://hengyud.cn/Gnuradio-UHD-OpenBTS-软件无线电平台搭建/#more))

[NodeJS v6.16.0(最好在6.10.0之后的版本)](https://nodejs.org/download/release/v6.16.0/)

```
# wget https://nodejs.org/download/release/v6.16.0/node-v6.16.0-linux-x86.tar.xz   
# tar xf  node-v6.16.0-linux-x86.tar.xz      
# cd node-v10.9.0-linux-x64/              
# ./bin/node -v    

ln -s /usr/software/nodejs/bin/npm   /usr/local/bin/ 
ln -s /usr/software/nodejs/bin/node   /usr/local/bin/
```
**pip install**

pip v19.1.1(`/usr/bin/pip`)
```
import sys
from pip import __main__
if __name__ == '__main__':
     sys.exit(__main__._main())
```
pip换源
```
pip install -i https://pypi.tuna.tsinghua.edu.cn/simple
或者
linux下，修改 ~/.pip/pip.conf (没有就创建一个)， 修改index-url至tuna，内容如下：
 [global]
 index-url = https://pypi.tuna.tsinghua.edu.cn/simple
windows下，直接在user目录中创建一个pip目录，如：C:\Users\xx\pip，新建文件pip.ini，内容如下
 [global]
 index-url = https://pypi.tuna.tsinghua.edu.cn/simple
```
tornado v4.4
Jinja2 v2.8
python-dateutil v2.8.0
PyYAML v5.1.1
numpy  v1.16.4
pandas v0.24.2
packaging v19.0
six v1.12.0
[bokeh v0.12.9(之后的版本移除了resize)](https://bokeh.pydata.org/en/0.12.9/docs/installation.html)
**apt install**

apt换源

```
sudo vim /etc/apt/sources.list

#deb包
deb http://mirrors.aliyun.com/ubuntu/ xenial main restricted universe multiverse 
deb http://mirrors.aliyun.com/ubuntu/ xenial-security main restricted universe multiverse  
deb http://mirrors.aliyun.com/ubuntu/ xenial-updates main restricted universe multiverse  
deb http://mirrors.aliyun.com/ubuntu/ xenial-backports main restricted universe multiverse 
# 源码  
deb-src http://mirrors.aliyun.com/ubuntu/ xenial main restricted universe multiverse  
deb-src http://mirrors.aliyun.com/ubuntu/ xenial-security main restricted universe multiverse  
deb-src http://mirrors.aliyun.com/ubuntu/ xenial-updates main restricted universe multiverse  
deb-src http://mirrors.aliyun.com/ubuntu/ xenial-backports main restricted universe multiverse
```
apache2
php7.0
mysql （mysql-server mysql-client）
libapache2-mod-php7.0
php7.0-mysql

**make**
[gr-bokehgui](https://github.com/kartikp1995/gr-bokehgui)


