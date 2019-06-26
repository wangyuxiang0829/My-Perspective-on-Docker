# Docker

## Docker基本组成

* Docker Client 客户端
* Docker Daemon 守护进程（服务器端）

>  客户端向守护进程也就是服务器端发送请求，守护进程处理完所有的工作并返回结果

* Docker Image 镜像
  * 构建和打包阶段

> 镜像是层叠的只读文件系统，最底层为引导文件系统(bootfs)，之上是root文件系统(rootfs)，可以是一种或多种操作系统

* Docker Container 容器
  * 通过镜像来启动
  * 启动和执行阶段
  * 写时复制(copy on write)

> 镜像是容器的基石，容器需要基于镜像启动和运行，镜像就好比容器的源代码，保存了用于启动容器的各种条件

* Docker Registry 仓库
  * 公有(Docker Hub)
  * 私有

> 仓库用于保存用户构建的镜像

