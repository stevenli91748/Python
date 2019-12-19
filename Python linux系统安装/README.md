

* 1 安装依赖包 
   
      首先安装gcc编译器，gcc有些系统版本已经默认安装，通过  gcc --version  查看，没安装的先安装gcc，
    
      [root]# yum -y install gcc
    
      安装其它依赖包，（注：不要缺少，否则有可能安装python出错，python3.7.0以下的版本可不装 libffi-devel
    
      [root]# yum -y install zlib-devel bzip2-devel openssl-devel ncurses-devel sqlite-devel readline-devel tk-devel gdbm-devel db4-devel libpcap-devel xz-devel libffi-devel
    
    
* 2 下载

      [root]# wget https://www.python.org/ftp/python/3.8.0/Python-3.8.0.tgz    
    
* 3  解压Python-3.8.0.tgz

      [root]# tar -zxvf Python-3.8.0.tgz    
      
* 4   建立一个空文件夹，用于存放python3程序

       [root]# mkdir /usr/local/python3
       
 * 5  执行配置文件，编译，编译安装　　　　　　　　　　　　

        [root]# cd Python-3.7.0
        [root]# ./configure --prefix=/usr/local/python3
        [root]#  make && make install      
