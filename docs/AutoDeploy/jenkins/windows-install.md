# windows下安装使用 jenkins

## 下载安装

进入[jenkins 官网](https://jenkins.io/zh/). 点击下载即可。

<div align=center>
	<img src="../images/img25.png" width="">
</div>

<div align=center>
	<img src="../images/img26.png" width="">
</div>

下载完成后，把安装包解压出来，按照指示安装即可。

<div align=center>
	<img src="../images/img42.png" width="">
</div>

## 端口配置

安装过程中要记住程序的安装路径，应为 jenkins 默认会占用 8080 端口，而 tomcat 的默认端口也是 8080，所以安装完成后要先修改 jenkins 的系统配置文件。

<div align=center>
	<img src="../images/img44.png" width="">
</div>

<div align=center>
	<img src="../images/img43.png" width="">
</div>

修改完成后重启 jenkins 服务让配置生效。

<div align=center>
	<img src="../images/img45.png" width="">
</div>

## 初始化配置

在网页上打开网址`http://<本地ip>:<刚刚修改的端口>/`出现如下界面

<div align=center>
	<img src="../images/img27.png" width="">
</div>

耐心等待一段时间后出现如下界面，根据路径提示找到系统生成的初始密码，点击继续

<div align=center>
	<img src="../images/img28.png" width="">
</div>

耐心等待，会出现插件安装提示，个人建议初学者选择默认

<div align=center>
	<img src="../images/img29.png" width="">
</div>

<div align=center>
	<img src="../images/img30.png" width="">
</div>

<div align=center>
	<img src="../images/img31.png" width="">
</div>

由于系统采用的是国外的源，导致插件安装特别慢，甚至失败，不用管点击继续

<div align=center>
	<img src="../images/img32.png" width="">
</div>

可以看到系统访问地址，点击继续

<div align=center>
	<img src="../images/img33.png" width="">
</div>

配置管理员用户及密码，点击继续进入jenkins初始界面

<div align=center>
	<img src="../images/img34.png" width="">
</div>

<div align=center>
	<img src="../images/img35.png" width="">
</div>


## 插件安装失败处理

选择Manage jenkins==>Manage Plugins==>更新中心，查看安装失败的插件

<div align=center>
	<img src="../images/img36.png" width="">
</div>

<div align=center>
	<img src="../images/img37.png" width="">
</div>

<div align=center>
	<img src="../images/img39.png" width="">
</div>

查看插件安装失败类型，绝大多数的下载失败或者因为某个插件下载失败导致其他依赖该插件的插件安装失败

<div align=center>
	<img src="../images/img41.png" width="">
</div>

下载失败的可以将错误信息的url复制到迅雷中下载（亲测可用）。或者用别人已经下载好的jpi安装文件通过上传安装。分享一下我的安装包
```
链接: https://pan.baidu.com/s/1yYNWlcwVXnsqaNFg5nmLkw 提取码: uuut
```

<div align=center>
	<img src="../images/img46.png" width="">
</div>

将默认插件安装好之后jenkins在windows系统下的安装配置算是基本完成了。