## Git 기초 실습 - 문제풀기

> 아래에 있는 각각의 문제에 대해 답과 이유를 작성하시오.
> 한 문제를 풀 때 마다 커밋을 저장하시오. 커밋 메시지는 "solve 문제번호 problem"의 형태로 저장하시오.

1. Git과 Github는 같다. (맞으면 O, 틀리면 X)

   - 답 : X
   - 이유 : platform

2. 터미널 명령어 `cd .`은 현재 위치의 부모 폴더로 이동하라는 의미이다. (맞으면 O, 틀리면 X)

   - 답 : X
   - 이유 : none

3. 마크다운 문법에서 글씨의 크기를 키우고 싶다고해서 본문을 제목으로 지정하면 안된다. (맞으면 O, 틀리면 X)

   - 답 : O
   - 이유 : hard to config

4. Git의 3가지 공간에는 Working Directory, Staging Area, Commits이 있다. (맞으면 O, 틀리면 X)

   - 답 : X
   - 이유 : commits to repository

5. Commit ID는 중복 가능하다. (맞으면 O, 틀리면 X)
   - 답 : O
   - 이유 :

# TIL Day 01

> 2022년 05월 19일 목요일

## Why Git & Github?

![img](https://user-images.githubusercontent.com/49775540/168756716-68f9aebb-380f-4897-8141-78d8403f6113.png)

### Git

- 분산 버전 관리 프로그램
- 백업, 복구, 협업을 위해 사용
- Git 공식문서 https://git-scm.com/book/ko/v2

### Github

- Git을 사용하는 프로젝트의 협업을 위한 웹호스팅 서비스
- 포트폴리오를 자랑할 수 있는 공간
- 1일 1커밋 하기
- 이동욱님 Github 계정 https://github.com/jojoldu

---

### CLI

> CLI (Command Line Interface, 커맨드 라인 인터페이스)는 터미널을 통해 사용자와 컴퓨터가 상호 작용하는 방식을 뜻한다.

#### 터미널 명령어 정리

| Command |                Explane                 |
| :-----: | :------------------------------------: |
|  mkdir  |      Make directory (folder only)      |
|  touch  | Create directory (extension mandatory) |
|   ls    |             Show file list             |
|   cd    |            Change directory            |
|   rm    |            Remove directory            |
|   pwd   |      Show current directory path       |
|   cwd   |            Remove directory            |

#### 예시

```bash
$ mkdir test

$ touch a.txt

$ ls
$ ls -a

$ cd ..
$ cd test

$ rm a.txt
$ rm -r test
```

### Visual Studio Code

> Visual Studio Code (비주얼 스튜디오 코드)는 마이크로소프트에서 개발한 텍스트 에디터의 한 종류이다.

#### 장점

- Windows, Mac, Linux 운영체제를 모두 지원한다.
- 기존 개발 도구보다 빠르고 가볍다.
- Extension을 통해 다양한 기능을 설치할 수 있어서, 무한한 - 확장성을 가진다.
- 무료로 사용 가능하다.

#### Git Bash 연동하기

1. 터미널을 연다. (Ctrl + `)
2. 화살표를 누르고 Select Default Profile을 클릭한다.
3. Git Bash를 선택한다.
4. 휴지통을 눌러서 터미널을 종료하고, 재시작한다.
   - 휴지통은 Kill Terminal 로써, 터미널 자체를 아예 종료한다.
   - 닫기는 Close Terminal 로써, 터미널을 종료하지 않고 창만 보이지 않게 만든다.
5. 기본 터미널이 Git Bash로 열리는지 확인한다.

### Markdown

> Markdown (마크다운)은 일반 텍스트 기반의 경량 Markup (마크업) 언어이다.

#### Markup (마크업) 이란?

- 마크(Mark)로 둘러싸인 언어를 뜻한다. 마크란 글의 역할을 지정하는 표시이다.
- HTML도 마크업 언어인데, 글에 제목의 역할을 부여할 때 `<h1>제목1</h1>` 과 같이 작성한다.

#### 마크다운의 장점과 단점

---

1. 장점
   - 문법이 직관적이고 쉽다.
   - 지원 가능한 플랫폼과 프로그램이 다양하다.
2. 단점
   - 표준이 없어서 사용자마다 문법이 상이하다.
   - 모든 HTML의 기능을 대신하지는 못한다.

#### 주의 사항

- 마크다운의 본질은 글에 역할을 부여하는 것이다.
- 반드시 역할에 맞는 마크다운 문법을 작성한다. 글씨를 키우고 싶다고 해서 본문에 제목의 역할을 부여하면 안된다.

---

#### 참고 자료

- [Markdown Guid](https://www.markdownguide.org/basic-syntax)
- [마크다운 문법 정리](https://gist.github.com/ihoneymon/652be052a0727ad59601)

# Git 3공간

- working dierctory
- staging
- repository

1. git init(dir 당 한번, 최상위 바탕화면에서 하지 말기)
2. git stauts
3. git add (staging, index added)
4. git commit -m "Comment"
5. config 설정
