
*****************gcc版本降到4.8*************************************
sudo update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-4.8 100
sudo apt-get install gcc-4.8
sudo update-alternatives --config gcc
gcc --version

**************安装依赖库***********************
 wget https://github.com/mongodb/mongo-c-driver/releases/download/1.13.1/mongo-c-driver-1.13.1.tar.gz
 tar xzf mongo-c-driver-1.13.1.tar.gz
 cd mongo-c-driver-1.13.1
 mkdir cmake-build
 cd cmake-build
 cmake -DENABLE_AUTOMATIC_INIT_AND_CLEANUP=OFF ..

 sudo apt-get install libssl-dev
 sudo apt-get install sqlite3
 sudo apt-get install libsqlite3-dev
 sudo apt-get install libevent-dev
 sudo apt-get install libpq-dev
 sudo apt-get install mysql-client
 sudo apt-get install libmysqlclient-dev
 sudo apt-get install libhiredis-dev