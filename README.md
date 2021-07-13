# smart-operation-management-api
致力于打造一个无侵入的云原生智能运维管理系统API

系统设计思路:

如果要打造一个无侵入的云原生智能运维管理系统,首先要解决的几大问题：

1. 远程服务器的认证登陆

远程服务器的认证登陆支持两种, 账号密码登陆和SSH KEY 密钥对方式进行登陆操作远程服务器,还要设置支持白名单和黑名单的支持。

2. 系统架构

系统设计采用前后端分离,UI 使用vue-element-admin,API 采用微服务架构可插拔式架构设计,方便API扩展。

3. SHELL 命令操作和文件上传功能

目前调研可选支持库有:

- Apache Commons Net

- JSch

- sshj

4.脚本库

- *.sh 脚本

- Spring Batch

5. 操作系统必须有一个统一的系统镜像

Tips: 所有的脚本要根据操作系统进行适配。

6. 所有软件安装使用脚本来执行且附带测试和操作日志功能

7. 脚本如何执行？

一种设计思路是类似Jenkins在要操作的服务器上部署Jenkins 这种对系统侵入性太强.

另外一种设计思路是上传脚本, 运维管理系统远程操作命令执行脚本。
