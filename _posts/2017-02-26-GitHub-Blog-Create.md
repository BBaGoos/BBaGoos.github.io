---
layout: post
title: 윈도우에서 jekyll로 GitHub Blog 만들기
---

MAC에선 크게 문제가 없었는데 역시나 Windows에선 환경 셋팅 및 설치가 복잡하다..
까먹기전에 후딱 포스팅하자.

## Windows에서 Jekyll설치 방법.

jekyll을 쓰기위해선 ruby,python 등 스크립트언어가 깔려있어야하는데 맥은 기본적으로 설치되어 있고 윈도우에선 따로 설치를 해줘야한다.
그리고 반드시 윈도우 계정을 **영어**로..**영어로** 하자.
윈도우 계정명이 한글이면 나중에 Pygments설치시 에러난다.

* 일단 [Ruby](http://rubyinstaller.org/downloads/) 와 [DevKit](http://rubyinstaller.org/downloads/)을 본인 OS에 맞춰서 다운 받아서 설치하자.

  * Ruby 설치시 아래 처럼 체크를 해줘야 cmd창 어디서든 ruby를 실행 할 수 있다.
  
  <div align="center">
  <img src="/public/img/ruby_install.jpg" />
  </div>
 
  * DevKit은 설치 후 CMD창에서 초기화 및 ruby와 binding을 해주자.
  * cd "Devkit설치 경로"
  * ruby dk.rb init
  * ruby dk.rb install
  * CMD화면 마지막에 [INFO] Installing ~~ 어쩌고 나오면 완료.

* 다음은 Jekyll설치.. Ruby의 gem 패키지 인스톨러를 이용해 설치.
  * CMD창에서 gem install jekyll
  * 뭐 권한 어쩌고 창뜨면 그냥 확인.
  * Done Installing documentation 어쩌고 나오면 완료.
 
* code blocks를 사용하기 위해 rouge 설치.
  * CMD창에서 gem install rouge
  * 역시나 Done Installing documentation 어쩌고 나오면 완료.
 
* Syntax highlighter를 쓰기위해 [Python](https://www.python.org/downloads/) 설치 (설치경로 확인하자).
  * 파이썬 설치 후 시스템 환경 변수 추가. 
  * 시스템 환경 변수 중 path에 아래 추가. 이건 PC마다 다를수 있으니 파이썬이 설치된 경로를 잘 알아 두자.
  * c:\Users\Administrator\AppData\Local\Programs\Python\Python36-32;c:\Users\Administrator\AppData\Local\Programs\Python\Python36-32\Scripts;
  * 정상적으로 설치/환경변수 등록이 완료되면 CMD 에서 python 엔터!
  * pip 엔터!!

* 다음은 위에 설치한 pip를 이용해 Pygments 설치.
  * CMD창에서 pip install Pygments
  * 위에서 말했지만 윈도우계정이 **한글** 이면 에러나니 설치가 안되면 윈도우 계정명을 **영어**로 바꾸자.
 
* 이제 설치가 끝났다.. 정상적으로 설치가 됐다면..CMD창에 명령어를 써보자
  * jekyll
  * jekyll 버전, 옵션 이런거 나오면 성공!!







