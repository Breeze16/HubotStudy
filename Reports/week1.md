# 第一周     Hubot与Slack的安装与连接

## 一、实训进度
本周安装了nodejs，Hubot和Slack，并完成了Hubot与Slack的连接。
## 二、遇到的问题
虽然本周内容比较简单，但是我在安装过程中遇到了很多问题。下面主要梳理一下遇到的问题。
### 1. 安装Hubot：权限问题
在执行命令“yo hubot”的时候，出现下图错误提示：
![](https://github.com/Breeze16/HubotStudy/blob/master/pictures/yo_error.png)                         
根据错误提示，是打开某文件夹权限出问题了。我去找了具体的文件夹，发现权限是root下，于是我使用chmod改变了权限组，解决了这个问题。
安装好Hubot后，出现了如下界面：
![](https://github.com/Breeze16/HubotStudy/blob/master/pictures/robot.png)
### 2. 安装Slack：翻墙问题
下载好Slack后，发现无法正常打开。想到老师有说需要翻墙，于是我下载了蓝灯。翻墙后成功打开了Slack桌面版。
### 3. 连接时出现的错误
将Hubot连接 到Slack上，需要在Slack上下载一个插件。下载好后，将其解压后放在了Hubot文件里。不过我现在没怎么搞懂这个插件应该如何用。
然后就是连接问题了。根据教程配置环境变量时，输入以下命令：，出现错误提示：body-parser deprecated undefined extended: provide extended option node_modules。查找了很多资料也没找到具体的解决办法。我刚开始输入的配置命令是：env HUBOT_SLACK_TOKEN=xoxb-582490373506-582410260944-3dgJTSFfpoDihwFEfjbpvVnU ./bin/hubot --adapter slack。后面根据老师的提示，将命令改成了：env HUBOT_SLACK_TOKEN=xoxb-582490373506-582410260944-3dgJTSFfpoDihwFEfjbpvVnU ./bin/hubot -a slack。试着运行了一下发现Slack上的Hubot可以正常使用了。如下图：
![](https://github.com/Breeze16/HubotStudy/blob/master/pictures/ping_pong.png)
### 4. 偶然发现系统源过期
在安装软件时发现自己ubuntu源过期了，具体提示是“定位不到软件包”。去网上找了清华大学的源连接，更改sources.list后成功。
