## docker常用命令

### 第一部分：镜像

本地镜像

```
docker images
```

搜索镜像

```
docker search  <image_name>
```

获取镜像

```
docker pull <image_name>

注：默认获取的为最新版本
```

获取指定版本镜像

```
docker pull <image-name>:<version-number>
```

从其他注册服务器仓库获取镜像

```
docker pull <host>:<port>/<image-name>
```

给镜像添加标签

    `docker tag <old-repository>/<old-tag> <new-repository>/<new-tag>`

### 第二部分：容器

运行中容器

`docker ps`

所有容器

`docker ps -a`

删除容器

`docker rm <container-id>|<container-name>`

注：参数为容器的ID或者容器的Name

启动/关闭/重启容器

`docker start/stop/restart <container-id>|<container-name>`
