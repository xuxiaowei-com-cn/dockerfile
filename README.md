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

1. [阿里巴巴 开源 JDK 8 项目 dragonwell8 docker 镜像](https://gitee.com/xuxiaowei-com-cn/dragonwell8.git)
2. [阿里巴巴 开源 JDK 11 项目 dragonwell11 docker 镜像](https://gitee.com/xuxiaowei-com-cn/dragonwell11.git)
3. [阿里巴巴 开源 JDK 17 项目 dragonwell17 docker 镜像](https://gitee.com/xuxiaowei-com-cn/dragonwell17.git)
4. [龙蜥 Anolisos git docker 镜像](https://gitee.com/xuxiaowei-com-cn/git.git)
5. [registry.gitlab.com/gitlab-org/gitlab-runner/gitlab-runner-helper Docker 镜像 hub.docker.com 站点](https://gitee.com/xuxiaowei-com-cn/gitlab-runner-helper.git)
6. [龙蜥 Anolisos Subversion（SVN） docker 镜像](https://gitee.com/xuxiaowei-com-cn/svn.git)

## 子模块 submodule

### 为何使用Git子模块？

1. 不同时间创建的仓库

```shell
git submodule add -b main ../dragonwell8.git dragonwell8
git submodule add -b main ../dragonwell11.git dragonwell11
git submodule add -b main ../dragonwell17.git dragonwell17
git submodule add -b main ../git.git git
git submodule add -b main ../gitlab-runner-helper.git gitlab-runner-helper
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

## 批量推送到远端仓库

<details>
<summary>点击展开</summary>

git fetch "origin" main:main

cd dragonwell8

git fetch "gitee" main:main

git.exe push --all --progress "gitee"

git.exe push --all --progress "gitlab"

git.exe push --all --progress "jihulab"

git.exe push --all --progress "github"

git.exe push --all --progress "gitcode"

git.exe push --all --progress "gitlink"

cd ..

cd dragonwell11

git fetch "gitee" main:main

git.exe push --all --progress "gitee"

git.exe push --all --progress "gitlab"

git.exe push --all --progress "jihulab"

git.exe push --all --progress "github"

git.exe push --all --progress "gitcode"

git.exe push --all --progress "gitlink"

cd ..

cd dragonwell17

git fetch "gitee" main:main

git.exe push --all --progress "gitee"

git.exe push --all --progress "gitlab"

git.exe push --all --progress "jihulab"

git.exe push --all --progress "github"

git.exe push --all --progress "gitcode"

git.exe push --all --progress "gitlink"

cd ..

cd git

git fetch "gitee" main:main

git.exe push --all --progress "gitee"

git.exe push --all --progress "gitlab"

git.exe push --all --progress "jihulab"

git.exe push --all --progress "github"

git.exe push --all --progress "gitcode"

git.exe push --all --progress "gitlink"

cd ..

cd gitlab-runner-helper

git fetch "gitee" main:main

git.exe push --all --progress "gitee"

git.exe push --all --progress "gitlab"

git.exe push --all --progress "jihulab"

git.exe push --all --progress "github"

git.exe push --all --progress "gitcode"

git.exe push --all --progress "gitlink"

cd ..

cd svn

git fetch "gitee" main:main

git.exe push --all --progress "gitee"

git.exe push --all --progress "gitlab"

git.exe push --all --progress "jihulab"

git.exe push --all --progress "github"

git.exe push --all --progress "gitcode"

git.exe push --all --progress "gitlink"

cd ..

git.exe fetch -v --progress "origin"

git.exe push --all --progress "origin"

</details>
