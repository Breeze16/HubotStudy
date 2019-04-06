# 第二周     安装配置Ansible

## 一、实训进度
本周安装配置了ansible
## 二、遇到的问题
（1）连接localhost成功，但是连接另一个组员时出现图二错误。这个错误老师也说没有遇到过，可能跟我的ubuntu版本或者ansible版本有关。暂时没有相关的解决办法。不过我组员的电脑可以成功连接到我这边，故而在后续开发中不会影响，因此这个问题被搁浅了。                    
![](https://github.com/Breeze16/HubotStudy/blob/master/pictures/success.png)           
![](https://github.com/Breeze16/HubotStudy/blob/master/pictures/Unreacheable.png)      
图一：连接本地成功;图二：连接外网失败。                 
（2）配置ssh时，无法连接到另一个组员的IP。后来发现是我们没在一个网段上。
（3）配置ssh时，即使在同一网段仍然无法成功连接。原因：ssh默认拒绝root用户连接。解决办法：通过 cat 等指令查看 /etc/ssh/sshd_config 中将PermitRootLogin no改为yes。
