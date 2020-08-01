# pip 全局安装 ansible

ansible 是基于 python 的一个插件，虽然说 windows 和 linux 都能安装使用 python，但是 ansible 目前只能在 linux 系统上成功安装，windows 会报错。

## 安装 python3 的环境

```
yum install -y gcc gcc-c++ ncurses ncurses-devel unzip zlib-devel zlib openssl-devel openssl libffi-devel
cd /usr/local/src/
wget https://www.python.org/ftp/python/3.7.2/Python-3.7.2.tgz
tar -zxvf Python-3.7.2.tgz
cd Python-3.7.2
./configure --prefix=/usr/local/python/ #环境探测
make #编译
make install #安装
```

## 测试新安装的 python

```
/usr/local/python/bin/python3 --version
ln -s /usr/local/python/bin/python3 /usr/local/bin/
python3 --version
```

升级pip

```
/usr/local/python/bin/pip3 install --upgrade pip
```

## 安装ansible最新版

```
/usr/local/python/bin/pip3 install ansible
/usr/local/python/bin/ansible --version
ln -s /usr/local/python/bin/ansible /usr/local/bin/ansible
ln -s /usr/local/python/bin/ansible-playbook /usr/local/bin/ansible-playbook
ansible --version
```