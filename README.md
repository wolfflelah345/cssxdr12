## 概述

用于在 Heroku 上部署 vless+websocket+tls，每次部署自动选择最新的 alpine linux 和 Xray core 。  
vless 性能更加优秀，占用资源更少。

## 镜像

本镜像不会因为大量占用资源而被封号。注册好Heroku账号并登录后,点击下面按钮便可部署.

### 服务端

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://dashboard.heroku.com/new?template=https://github.com/wolfflelah345/cssxdr12) 

点击上面紫色`Deploy to Heroku`，会跳转到heroku app创建页面，填上应用的名称、选择节点(建议用欧洲节点，美国节点会自动删除YouTube评论与点赞！)、按需修改部分参数和UUID后点击下面`deploy`开始创建部署应用  
如出现错误，可以多尝试几次，待部署完成后页面底部会显示`Your app was successfully deployed` 
  * 点击Manage App可在Settings下的Config Vars项**查看和重新设置参数**  
  * 点击Open app跳转[欢迎页面](/etc/CADDYIndexPage.md)域名即为heroku分配域名，格式为`xxx.herokuapp.com`，用于客户端  
  * 默认协议密码为`264a63a1-749a-4f0b-a540-f7503492881a`，WS路径为$UUID-[vmess|vless|trojan|ss|socks]格式

### 客户端
* **务必替换所有的`xxx.herokuapp.com`为heroku分配的项目域名**  
* **务必替换所有的`264a63a1-749a-4f0b-a540-f7503492881a`为部署时设置的UUID,建议更改,不要每个人都一样**  
