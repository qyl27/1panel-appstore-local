# 1Panel 本地应用商店

[1Panel](https://github.com/1Panel-dev/1Panel)  应用商店的本地存储库，收录一些可能会被用到但官方商店未收录的项目。

（欢迎 PR 。）

## 食用方法

### 1、Clone 本仓库到你喜欢的位置

```shell
git clone https://github.com/qyl27/1panel-appstore-local.git
```

### 2、软连接存储库内的 `local` 目录到 1panel 的 `./resources/apps/local` 

```shell
ln -s ./local /opt/1panel/resource/apps/local
```

### 3、在 1panel 中勾选显示本地应用，并刷新应用列表

### 4、日常从 GitHub 上拉取最新提交

```shell
git pull
```

## 驾照

继承自 [1panel-dev/appstore](https://github.com/1Panel-dev/appstore) 的 GPLv3。

## Todo

- [ ] 自动化接收上游软件 Docker 镜像更新。

