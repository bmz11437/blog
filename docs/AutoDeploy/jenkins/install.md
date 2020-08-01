# centos7 环境下部署 Jenkins

## 安装 weget

```
 yum install wget -y
```

## 安装 jenkins yum 源

```
  wget -O /etc/yum.repos.d/jenkins.repo http://pkg.jenkins.io/redhat-stable/jenkins.repo
```

## 下载并导入 yum 仓库的 key

```
  rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io.key
```

## 安装 java 环境

```
 yum install java -y
```

## 安装 Jenkins

```
  yum install jenkins -y
```

## 创建 deploy 用户作为系统服务用户

```
  vi /etc/sysconfig/jenkins
```
