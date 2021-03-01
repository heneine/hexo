---
title: "Git 기본 사용법"
date: 2020-08-07T00:10:45+09:00
draft: true
doc: true
---
#GIT 기본 명령어

git을 처음 접했을 때 주로 이용하는 일부 명령어만 담았습니다.
</br></br>

### git init

```bash
$ git init
```
현재 위치한 경로에 로컬 저장소를 만든다.
</br>

### git init

```bash
$ git remote add origin https://github.com/사용자명/레파지토리명.git
```
현재 위치한 로컬저장소와 기입한 주소인 원격저장소를 연결한다.
이제부터 로컬저장소를 통해 원격저장소를 관리할 수 있다.
</br>

### git add

```bash
$ git add <파일명>
```
git이 파일을 추적하도록 한다.
파일명 위치에 .을 적으면 현재 위치한 디렉토리의 모든 파일을 추적한다.
</br>

### git commit

```bash
$ git commit -m "Message"
```
git add로 추적중인 파일을 커밋한다.
커밋 메세지는 "Message"자리에 기입한다.
</br>

### git push

```bash
$ git push origin master
```
git push는 커밋한 파일을 원격저장소(Github)에 업로드하는 명령어이다.
뒤에 origin은 오리지널이라는 의미로 원격저장소를 의미하며, master은 [브랜치](https://backlog.com/git-tutorial/kr/stepup/stepup1_1.html)이다.
해당 명령어를 사용하려면 git remote를 통해 로컬저장소와 원격저장소를 연결해줘야 한다.
</br>

## vim 에디터
```bash
$ vim <파일명>
```
텍스트 에디터이다.
문서를 열고 i(insert)를 누르면 수정이 가능하다.
수정을 마치면 ESC를 누르고 :wq를 입력한다. (w:저장, q:나가기)
