---
layout: post
title:  Github Page 만들기 (w/jekyll minima)
date:   2023-03-15 13:40:49 +0900
categories: jekyll update
---
앞으로는 잘 기록해두는 것이 좋을 것 같아, 블로그를 시작해보려고 한다.
대표적으로 사용되는 블로그 플랫폼 중 Github Page를 사용해 보기로 했다. 
페이지를 직접 만들어볼 수 있어서, 그 과정에서 GitHub도 익숙해 질 수 있을 것 같다. 오늘 작업한 내용을 살펴 보면,
<br><br>

1. **Git repository 만들고, 로컬에 복사하기**
* Git   
        * <a href="https://docs.github.com/ko/repositories/creating-and-managing-repositories/cloning-a-repository" target="_blank">GitHub repository 복사</a>  
        * <a href="https://pages.github.com/" target="_blank">GitHub Pages</a>     
* Brew   
        * 오픈 소스 패키지 관리 시스템, macOS 운영 체제의 소프트웨어 설치를 단순하게 만들어준다.         
* Ruby     
        * 오픈 소스 프로그래밍 언어, 프로그래머의 단짝 친구    
        * <a href="https://jekyllrb-ko.github.io/docs/ruby-101/" target="_blank">루비 기초</a>
        * <a href="https://www.ruby-lang.org/ko/" target="_blank">Ruby</a>  
<br>
2. **jekyll admin page 만들기(CMS)**
    - Gem     
        * 루비 프로젝트를 JSON으로 변환
        * 페이지 나누기, GitHub API 연동      
    - Gemfile     
        * Gem 파일 목록     
    - Bundler     
        * Gemfile에 있는 젬들 설치     
    - Liquid      
        * (오브젝트, 태그, 필터)      
    - 상단에 루비 기초 참고
<br><br>
3. **jekyll minima theme 적용하고, 홈화면 레이아웃 커스터 마이징**<br>
    * Minima 설치 경로 확인
        > bundle show minima
    * 로컬에 디렉토리 생성
        > mkdir -p ./_layouts
    * home.html 파일 복사
        > cp Minima 경로/_layouts/home.html ./_layouts/
<br><br>
4. **마크다운 기본 문법 찾아보기**
<br><br>
5. **첫 포스트 올리기** <br>

    * 터미널 입력 관련    
        > git add .    
        > git commit -m "message"    
        > git push    
        > bundler exec jekyll serve     
        > ⌃c 

<br><br><br>
이렇게 만들고나니 jekyll의 기본 테마인 minima도 깔끔한 것 같다. 앞으로 사용하면서 필요한 것들 위주로 맞춰나가면 좋을 것 같다.
<br><br><br>
etc.
<ul>
    <li>처음엔 jekyll을 제키-투로 읽었다. 지킬로 읽는 듯 하다.</li>
    <li>Brew / Ruby / GitHub / Jekyll 를 좀 더 알아보면 좋을 것 같다.</li>
    <li>디렉토리 관리 및 파악 중요</li>
    <li>버전 관리 및 파악 중요</li>
</ul>
<br>
Next To Do
<ul>
<li>Default 폰트 세팅 확인</li>
<li>모바일 버전 레이아웃 확인</li>
<li>메뉴 카테고리 추가</li>
<li>파비콘, OG 이미지 추가</li>
</ul>

<br><br>
<hr style="border-width:0.5px">
<br>
:: 참고    
<a href="https://pages.github.com/" target="_blank">GitHub Pages</a>  
<a href="https://jekyllrb-ko.github.io/docs/" target="_blank">Jekyll Docs</a>     
<a href="https://talk.jekyllrb.com/" target="_blank">Jekyll Talk</a>     
<a href="https://labs.brandi.co.kr/2018/05/14/chunbs.html" target="_blank">jekyll을 이용한 Github 블로그 만들기(추천)</a>    
<a href="https://martinkang.github.io/develop/2022/03/26/blog-base-html-layout.html" target="_blank">코딩 독학</a>      
<a href="https://gist.github.com/ihoneymon/652be052a0727ad59601" target="_black">마크다운(Markdown 사용법)</a>     



