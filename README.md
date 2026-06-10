<div align="center">

<img src="https://voidlinux.org/assets/img/void_bg.png" width="75" />

<h1>Custom XBPS Void Linux Repository</h1>

[![Build](https://img.shields.io/github/actions/workflow/status/grvn/void-packages/build.yml?style=for-the-badge&label=BUILD&logo=githubactions&logoColor=white)](https://github.com/grvn/void-packages/actions)
&nbsp;
[![Updates](https://img.shields.io/github/actions/workflow/status/grvn/void-packages/update.yml?style=for-the-badge&label=AUTO-UPDATE&logo=github&logoColor=white)](https://github.com/grvn/void-packages/actions)


### 1. Add the repository

```shell
printf "repository=https://github.com/mojamuto/void-repo/releases/latest/download\n" | sudo tee /etc/xbps.d/10-mojamuto-repo.conf
```

### 2. Sync and trust the signing key

```shell
xbps-install -S
```

> *__NOTE__*: First time running `xbps-install -S` you will be asked if you wish to import the repository key.


### 3. Repo is ready to use

#### 🔄 Updates?

Once the repo is added, package updates will come automatically with:
```shell
xbps-install -Su
```

> *__NOTE__*: Muchas gracias a grvn por su repositorio: [![Link](https://github.com/grvn/void-packages)
