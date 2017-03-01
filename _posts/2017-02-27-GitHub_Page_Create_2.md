---
layout: post
title: 윈도우에서 jekyll로 GitHub Blog 만들기 (2)
categories: [blog, jekyll]
tags: [jekyll,GitHub Page]
---

뭐지... 날라갔네... OTL
다시 급하게 후딱 마무리 하자.


* GitHub가입 Repository생성 

  * GitHub 가입 후 Start a Project 클릭
  
  <div align="center">
  <img src="/public/img/git1.jpg" />
  </div>
  
  * Repository name은 `Owner명.github.io`
  
  <div align="center">
  <img src="/public/img/git2.jpg" />
  </div>
  
  * 이렇게만들면 추후 브라우져에서 Owner명.github.io 로 접속 할 수 있다.
  * Create Repository 클릭.
  
* [Windows용 Git](http://git-scm.com/download/) 다운받고 설치.  
  * 설치는 어렵지 않다 그냥 무조건 다음다음다음 
  
  
* jekyll로 Local Repository만들기.
  * CMD창에서 Local Repository를 만들 위치까지 이동.
  * `jekyll new Owner명.github.io`
  * `jekyll serve -w`
  * 뭔가 Compress 되고 Server running... press ctrl-c to stop. 나오면 성공.
  * 이제 브라우저에서 http://localhost:4000 으로 접속. 페이지 나오면 성공.
  
* Local Repository와 원격 Repository 연동.
  * CMD창에서 Local Repository 경로까지 진입 후 
  * `git config --global user.name "owner명"`
  * `git config --global user.email "github 가입 Email"`
  * `git init`
  * `git remote add origin https://github.com/owner명/Owner명.github.io.git`
  * `git add .`
  * `git commit -m "커밋 로그 커맨트"`
  * `git push origion master`
  * 잠시 후 브라우저에서 Owner명.github.io.git 접속하면 아까 localhost에서 봤던 화면이 보이면 성공.
  
다쓰고 올렸는데 왜.... 포스팅 파일이 날라갔을까.. 휴.
무튼 이렇게 해서 jekyll과 GitHub Page로 블로그 만들기 성공!
다음은 테마 적용과 포스팅하는 방법에 대해 포스팅 할 예정!







