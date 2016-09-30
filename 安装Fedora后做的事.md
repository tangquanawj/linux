## 安装Fedora24后该作的几件事

#### 第一.更新系统
    sudo dnf update

#### 第二.将新建的用户添加到su用户组
新安装好的Fedora默认用户是不在sudo用户组的，当你执行sudo命令时，会提醒你当前用户并不在sudo用户组里面。此时可以采取下面措施，将当前你的用户加入sudo用户组，配置好后即可使用sudo命令.

* 1.首先切换到 root。
* 2.然后vim /etc/sudoer，在root ALL=(ALL) ALL的下面添加  tang ALL=(ALL)  ALL 。
* 3.wq保存文件即可。
* 4.测试是否正确配置了sudo，只需要在普通用户权限下输入$sudo whoami。配置正确，命令就会返回root字样。

#### 第三.安装Guake下拉命令栏
命令行执行：

    sudo dnf install guake
输入密码后即可

#### 第四.安装git，将此博文同步到Github，并同时提交到Hexo的个人博客

#### 第五.配置Hexo博客环境

#### 第六.浏览器安装flash player插件

#### 第七.安装conky系统检测软件

#### 第八.配置shadowsocks-qt5科学上网
	
	sudo dnf copr enable librehat/shadowsocks
	sudo dnf update
	sudo dnf install shadowsocks-qt5 
执行完上面的命令就装好了。具体的配置方法就很简单，不一一写了。

#### 第九.安装和配置Tweak Tools，设置所需程序开机自动启动。
* 打开软件中心，输入名字Tweak tools，安装即可。
* 运行Tweak Tools，选择Extensions。
* 点击Get more Extensions，从插件官网下载有用的插件。
* 下载Drop Down Terminal , Simple net Speed。
* 点击Tweak Tools的startup，添加guake为子启动程序。

#### 第十.安装virtualbox，并在其中安装Windows 7

* [VirtualBox](https://www.virtualbox.org/)

#### 第十.
