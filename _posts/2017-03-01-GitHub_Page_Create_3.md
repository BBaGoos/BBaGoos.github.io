---
layout: post
title: jekyll로 GitHub Blog 만들기 for windows (3)
categories: [jekyll]
tags: [jekyll,Github Blog,GitHub Page]
---

 원래는 theme 입히는걸 포스팅하려했으나 아직 좀더 공부하고 올려봐야겠다.
 그래서 이번 포스팅은 다른 PC에서 원격저장소에 있는 소스를 내려받아 셋팅하는 방법이다.
 

* Jekyll을 처음 설정한 PC가 아닌 다른 PC에서 소스 내려받아 작업하기. 

  * Ruby,Pythone,Bundle,GIT,Jekyll등은 미리 설치해둔다.
  * 셋팅 또한 이전 포스팅 내용을 보면서 [Github Blog 만들기(1)](https://gu-nine.github.io/blog/jekyll/2017/02/26/GitHub_Page_Create/),[Github Blog 만들기(2)](https://gu-nine.github.io/blog/jekyll/2017/02/27/GitHub_Page_Create_2/) 기본적인 셋팅을 한다.
  * CMD창에서 jekyll new 로 생성한 디렉토리로 이동 후 
  * `git remote add origin https://github.com/owner명/Owner명.github.io.git`
  * `git clean  -d  -fx ""`
  * `git pull origin master`
  
* Gem 으로 Bundle 설치.  
  * CMD창에서 `bundle install`

* Jekyll serve 명령어로 로컬에서 확인하기.
  * CMD창에서 `jekyll serve -w`
  * server running 메시지가 나오면 브라우저에서 `http://localhost:4000`
  
정상적으로 블로그가 뜬다면 끝!





