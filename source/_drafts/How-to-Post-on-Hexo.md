---
title: "Hexo로 블로그 포스팅하기"
date: 2020-08-07T00:44:53+09:00
draft: true
toc: true
---

## About Posting

### Writing

```bash
hexo new [layout] <title>
```
post는 기본 layout이다.
layout은 post, page, draft 가 있다.

---------
### Draft to Post

```bash
hexo publish [layout] <title>
```
Writing할 때 layout을 Draft로 설정했다면 source/_drafts 내부에 포스트가 생성될 것이다.
이를 publish를 통해 source/_post로 옮길 수있다.

--------

## Deploy & Git-Push

### Deploy

```bash
hexo generate
```
이 명령어를 실행하면 public 폴더가 생성되면서 정적 리소스가 생성된다.
이 파일들이 실제로 깃허브 페이지에 배포될 파일들이다.

```bash
hexo deploy
```
hexo generate를 통해 생성한 정적 리소스를 배포한다.
_config.yml에서 사전에 설정한 주소로 배포된다.

```bash
hexo deploy
```
정적 리소스를 삭제하는 명령어이다.
간혹 정상적으로 배포가 되었음에도 불구하고 페이지가 업데이트 되지 않는 현상이 있는 경우 사용하면 된다.

```bash
hexo deploy --generate
```
정적 리소스 및 배포를 동시에 할 수 있다.

---------

### Git Push

```bash
git add .
git commit -m "Message"
git push origin master
```
깃허브 저장소에 소스를 저장한다.
(자세한건 Github-Basic-Guide 포스팅 참조)

~~git push origin master 가 안될 경우, git push -f origin master을 이용한다. (f는 force)~~ ~~잘몰라~~
