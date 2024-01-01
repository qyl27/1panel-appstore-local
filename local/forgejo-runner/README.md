# Forgejo Runner

用于执行 Forgejo Actions 的 Runner 。



**请先注册 Runner ，再安装此应用。**

## 注册 Runner

交互式注册：

```shell
docker run -it --rm \
  -v forgejo_runner_data:/data \
  code.forgejo.org/forgejo/runner:3.3.0 \
  forgejo-runner register
```
