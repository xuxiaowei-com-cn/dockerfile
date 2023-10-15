<div align="center" style="text-align: center;">
    <h1>Dockerfile</h1>
    <h3>Dockerfile（git 父模块）</h3>
    <a target="_blank" href="https://github.com/996icu/996.ICU/blob/master/LICENSE">
        <img alt="License-Anti" src="https://img.shields.io/badge/License-Anti 996-blue.svg">
    </a>
    <a target="_blank" href="https://996.icu/#/zh_CN">
        <img alt="Link-996" src="https://img.shields.io/badge/Link-996.icu-red.svg">
    </a>
    <a target="_blank" href="https://qm.qq.com/cgi-bin/qm/qr?k=ZieC6s1WB4njfVbrDHYgoNS8YpT26VtF&jump_from=webapi">
        <img alt="QQ群" src="https://img.shields.io/badge/QQ群-696503132-blue.svg"/>
    </a>
</div>

<p></p>

<div align="center" style="text-align: center;">
    <a target="_blank" href="https://work.weixin.qq.com/gm/75cfc47d6a341047e4b6aca7389bdfa8">
        <img alt="企业微信群" src="static/wechat-work.jpg" height="100"/>
    </a>
</div>

1. [alpine-glibc](https://gitee.com/xuxiaowei-com-cn/alpine-glibc.git)
2. [centos7-glibc](https://gitee.com/xuxiaowei-com-cn/centos7-glibc.git)
3. [debian](https://gitee.com/xuxiaowei-com-cn/debian.git)
4. [docker-in-docker](https://gitee.com/xuxiaowei-com-cn/docker-in-docker.git)
5. [dragonwell](https://gitee.com/xuxiaowei-com-cn/dragonwell.git)
6. [阿里巴巴 开源 JDK 11 项目 dragonwell11 docker 镜像](https://gitee.com/xuxiaowei-com-cn/dragonwell11.git)
7. [阿里巴巴 开源 JDK 17 项目 dragonwell17 docker 镜像](https://gitee.com/xuxiaowei-com-cn/dragonwell17.git)
8. [阿里巴巴 开源 JDK 8 项目 dragonwell8 docker 镜像](https://gitee.com/xuxiaowei-com-cn/dragonwell8.git)
9. [龙蜥 Anolisos git docker 镜像](https://gitee.com/xuxiaowei-com-cn/git.git)
10. [gitlab-runner-helper](https://gitee.com/xuxiaowei-com-cn/gitlab-runner-helper.git)
11. [golang](https://gitee.com/xuxiaowei-com-cn/golang.git)
12. [golang-alpine-glibc](https://gitee.com/xuxiaowei-com-cn/golang-alpine-glibc.git)
13. [java](https://gitee.com/xuxiaowei-com-cn/java.git)
14. [keepalived](https://gitee.com/xuxiaowei-com-cn/keepalived.git)
15. [kube-state-metrics](https://gitee.com/xuxiaowei-com-cn/kube-state-metrics.git)
16. [metrics-server](https://gitee.com/xuxiaowei-com-cn/metrics-server.git)
17. [墨菲安全 murphysec docker 版](https://gitee.com/xuxiaowei-com-cn/murphysec.git)
18. [nginx](https://gitee.com/xuxiaowei-com-cn/nginx.git)
19. [node-dpkg-fakeroot-rpm](https://gitee.com/xuxiaowei-com-cn/node-dpkg-fakeroot-rpm.git)
20. [node-rpm](https://gitee.com/xuxiaowei-com-cn/node-rpm.git)
21. [prometheus-adapter](https://gitee.com/xuxiaowei-com-cn/prometheus-adapter.git)
22. [prometheus-webhook](https://gitee.com/xuxiaowei-com-cn/prometheus-webhook.git)
23. [阿里巴巴 面向云原生微服务的高可用流控防护组件 docker 版](https://gitee.com/xuxiaowei-com-cn/sentinel.git)
24. [svn](https://gitee.com/xuxiaowei-com-cn/svn.git)

## 子模块 submodule

### 为何使用Git子模块？

1. 不同时间创建的仓库

```shell
git submodule add -b main ../alpine-glibc.git alpine-glibc
git submodule add -b main ../centos7-glibc.git centos7-glibc
git submodule add -b main ../debian.git debian
git submodule add -b main ../docker-in-docker.git docker-in-docker
git submodule add -b main ../dragonwell.git dragonwell
git submodule add -b main ../dragonwell11.git dragonwell11
git submodule add -b main ../dragonwell17.git dragonwell17
git submodule add -b main ../dragonwell8.git dragonwell8
git submodule add -b main ../git.git git
git submodule add -b main ../gitlab-runner-helper.git gitlab-runner-helper
git submodule add -b main ../golang.git golang
git submodule add -b main ../golang-alpine-glibc.git golang-alpine-glibc
git submodule add -b main ../java.git java
git submodule add -b main ../keepalived.git keepalived
git submodule add -b main ../kube-state-metrics.git kube-state-metrics
git submodule add -b main ../maven-mysql-client.git maven-mysql-client
git submodule add -b main ../metrics-server.git metrics-server
git submodule add -b main ../murphysec.git murphysec
git submodule add -b main ../nginx.git nginx
git submodule add -b main ../node-dpkg-fakeroot-rpm.git node-dpkg-fakeroot-rpm
git submodule add -b main ../node-rpm.git node-rpm
git submodule add -b main ../prometheus-adapter.git prometheus-adapter
git submodule add -b main ../prometheus-webhook.git prometheus-webhook
git submodule add -b main ../sentinel.git sentinel
git submodule add -b main ../svn.git svn
```

## 克隆 clone

```shell
git clone https://gitee.com/xuxiaowei-com-cn/dockerfile.git --recursive
```

```shell
git clone https://gitee.com/xuxiaowei-com-cn/dockerfile.git
cd dockerfile
git submodule
git submodule init
git submodule update
```

## 更新 update

```shell
git submodule update
git submodule update --remote
```

## 批量切换分支

```shell
git submodule foreach git checkout main
```

## 批量添加远端仓库地址

<details>
<summary>点击展开</summary>
git remote add gitee https://gitee.com/xuxiaowei-com-cn/dockerfile.git
git remote add gitlab https://gitlab.com/xuxiaowei-com-cn/dockerfile.git
git remote add jihulab https://jihulab.com/xuxiaowei-com-cn/dockerfile.git
git remote add github https://github.com/xuxiaowei-com-cn/dockerfile.git
git remote add gitcode https://gitcode.net/xuxiaowei-com-cn/dockerfile.git
git remote add gitlink https://gitlink.org.cn/xuxiaowei-com-cn/dockerfile.git

# Windows 需要使用 git bash

git submodule foreach 'git remote add gitee https://gitee.com/xuxiaowei-com-cn/$(basename $path).git'
git submodule foreach 'git remote add gitlab https://gitlab.com/xuxiaowei-com-cn/$(basename $path).git'
git submodule foreach 'git remote add jihulab https://jihulab.com/xuxiaowei-com-cn/$(basename $path).git'
git submodule foreach 'git remote add github https://github.com/xuxiaowei-com-cn/$(basename $path).git'
git submodule foreach 'git remote add gitcode https://gitcode.net/xuxiaowei-com-cn/$(basename $path).git'
git submodule foreach 'git remote add gitlink https://gitlink.org.cn/xuxiaowei-com-cn/$(basename $path).git'
</details>
