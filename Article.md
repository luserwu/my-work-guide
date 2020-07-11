> ### 安装谷歌插件

Online-Tool  ->  在线工具  ->  Chrome插件下载  ->  下载需要的.crx文件修改为.rar或者其他压缩格式  ->  解压  ->  Chrome扩展程序打开开发者模式，加载已解压的扩展程序，选择上一步的解压文件即可。推荐： 
- Similar Sites  
- Octotree  
- SourceGraph  
- GitZip 
- OneTab  
- Momentum  
- 简悦  
- Smart PDF  
- My IP address  
- Talend API Tester  
- JSON Viewer Awesome  
- AdGuard AdBlocker  
- Extension Manager  
> ### idea插件  
 
- IDE Features Trainer  (IDEA交互式教程)  
- RestfulToolkit  (RESTful服务开发)  
- Key Promoter X  (快捷键)  
- Presentation Assistant  (快捷键展示)  
- Codota  (代码智能提示)  
- Alibaba Java Code Guidelines  (阿里巴巴Java代码规范)  
- GsonFormat+RoboPOJOGenerator  (JSON转类对象)  
- Statistic  (项目信息统计)  
- Translation  (必备的翻译插件)  
- CamelCase  (多种命名格式之间切换)  
- Grep Console  (控制台输出处理)
- Rainbow Brackets  (彩虹🌈括号)
- Save Actions  (优化保存操作)
- SequenceDiagram  (一键生成时序图)
- Maven Helper  (分析Maven项目的相关依赖)
- EasyCode  (一键帮你生成所需代码)
- CheckStyle  (代码格式检查)
- SonarLint  (帮你优化代码)
- Lombok  (帮你简化代码)
- CodeGlance  (代码微型地图)
- Java Stream Debugger  (Java8 Stream调试器)
- Git Commit Template  (使用模板创建commit信息)  
- A Search with Github  (通过 Github搜索相关代码)  
- stackoverflow  (快速跳转到 stackoverflow)  
- CodeStream  
- Code screenshots  (代码片段保存为图片)  

> ###docker

非root用户如何使用docker  
查看是否有docker用户组:sudo cat /etc/group | grep docker  
若无则创建用户组,并将用户添加进docker用户组:  
- sudo groupadd -g 999 docker(999为组id)  
- sudo usermod -aG docker domi  
重启docker生效:  
- sudo service docker restart(Ubuntu系统)
- sudo systemctl restart docker(Centos系统)  
需要/var/run/docker.sock权限:sudo chmod a+rw /var/run/docker.sock  
docker卸载镜像:
- 查看镜像进程:docker ps -a  
- 停止镜像进程:docker stop 容器id  
- 删除镜像进程:docker rm 容器id  
- 查看docker镜像:docker images  
- 删除docker镜像:docker rmi 镜像id  
- docker基础命令  
![](source/docker命令.png)  

>### 配置git  

- 配置git环境:  
git config --global user.name "你的用户名"
git config --global user.email "你的注册邮箱"  
- 生成SSH秘钥:  
ssh-keygen -C "你的注册邮箱" -t rsa  
- github配置公钥:  
setting填入生成的公钥(id_rsa.pub)  
- 将key加入ssh-agent:  
ssh-add  ~/.ssh/id_rsa
