# Forgejo Runner

用于执行 Forgejo Actions 的 Runner 。



**请先注册 Runner 并且启动 Docker in Docker，再安装此应用。**

## 注册 Runner

交互式注册：

```shell
docker run -it --rm \
  -v forgejo_runner_data:/data \
  code.forgejo.org/forgejo/runner:3.3.0 \
  forgejo-runner register
```



## 启动 Docker in Docker

```shell
docker network create forgejo_runner_network

docker run -it -d \
  --name forgejo_runner_docker_in_docker \
  --network forgejo_runner_network \
  --privileged \
  docker:dind \
  dockerd -H tcp://0.0.0.0:2375 --tls=false
```

