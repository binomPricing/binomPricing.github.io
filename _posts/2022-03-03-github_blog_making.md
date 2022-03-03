---
title: (Github 에서 jekyll 로) 블로그 만들기
tags:
- git
- blog
- ruby
- jekyll
categories:
- Programming
date: 2022-03-02 10:28:20
---

자기가 환경을 조정할 수 있는  
블로그 만드는 가장 편리한 방법 중 하나가  
Github 에서 jekyll 을 이용

# 먼저 git 사용환경 설정

반드시 git 필요한 것은 아니지만  
편리한 이용을 위해 실질적으로 필요

1. [Github](https://github.com/) 계정 만들어 원격 저장소 만들기

2. 자기 컴퓨터에서 git 환경(로컬 저장소) 만들기
    - 글로벌 설정하고 : git --global config
    - 프로젝트 폴더 만들어 
        - 로컬 설정 : git config 
        - 글로벌리 설정보다 우선하여 적용됨
        - 글로벌리 내용과 같으면 생략

# jekyll theme 정하여 받아오기

1. jekyll theme fork
    - [jekyll theme 싸이트](http://jekyllthemes.org/)에 가서  테마들 보기
    - 선택한 테마의 깃헙주소로 가서 자기 깃헙 저장소로 포크함
    - 국내 사용자들은 [minimal mistakes](https://mmistakes.github.io/minimal-mistakes/) 애용하는 듯
      - 이들 테마 홈페이지 하단에 보면 깃헙 저장소 연결 링크가 있음
      - 이들 테마 깃헙 저장소 우상단에 보면 포크 표시 있음

2. 프로젝트 폴더(로컬저장소)에 원격저장소 연결
    - git clone 또는 pull 등으로 내용 받아옴

# 로컬 서버 환경 구축

1. 로컬에 루비와 지킬 설치
    - [지킬 싸이트](https://jekyllrb-ko.github.io/docs/)에서 빠른 설치 참고
    - 로컬에서 웹페이지 실행
        - 명령 : bundle exec jekyll serve
        - 실행 결과 나타나는 URL 주소를 Ctrl + 클릭
        - 또는 브라우저에 디폴트 주소 입력
            - http://localhost:4000/

2. 로컬에서 내용 수정 및 결과 확인
    - 적절한 에디터 이용 : VS Code 권장
      - 해당 폴더에서 `code . ` 명령으로 VS Code 실행
    - 로컬에서 내용 저장 후 실시간 확인
      - 에디터 저장 후 로컬호스트 내용 갱신  

# 깃으로 로컬 수정 내용 원격에 반영

1. 로컬 수정 내용을 원격저장소에 반영
    - 로컬에서 git add >> commit >> push

2. 깃헙 인터넷 블로그 내용도 조금 뒤 수정됨
