# NCL安装

## 安装libssl.so.10

wget https://www.openssl.org/source/old/1.0.1/openssl-1.0.1e.tar.gz
tar zxvf ...
./config shared zlib-dynamic
cp libssl.so.1.0.0 /usr/lib64
cp libcrypto.so.1.0.0 /usr/lib64
cd /usr/lib64
ln -s libssl.so.1.0.0 libssl.so.10
ln -s libcrypto.so.1.0.0 libcrypto.so.10

添加环境变量
LD_LIBRARY_PATH = $LD_LIBRARY_PATH:/usr/lib64

## 安装libgfortran3

vi /etc/apt/sources.list
apt-get update
sudo apt-get install g++-6
sudo apt-get install libgfortran3

