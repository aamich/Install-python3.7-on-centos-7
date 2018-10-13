# Install-python3.7-on-centos-7
yum install gcc openssl-devel bzip2-devel libffi libffi-devel
cd /usr/src/
wget https://www.python.org/ftp/python/3.7.0/Python-3.7.0.tgz
tar xzf Python-3.7.0.tgz
cd Python-3.7.0/
./configure --enable-optimizations
make altinstall
ln -s /usr/local/bin/python3.7 /usr/bin/python3
rm /usr/src/Python-3.7.0.tgz
python3 -V
