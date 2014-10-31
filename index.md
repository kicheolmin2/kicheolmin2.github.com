---
layout: page
title: Hello!
tagline: Ki&Song's Blog
---
{% include JB/setup %}

## 안녕하세요

아두이노 관련 학습 블로그 입니다.
학습내용과 관련 퀴즈까지 준비했습니다.

블로그 사용법 :
    
    오른쪽 상단 버튼 : 홈, 카테고리, 테그
    
    왼쪽 바 :
      편지모양 : 이메일
      사람마크 : github 페이지
      feed : 최근 사용
      파란마크 : 홈버튼
    
## 포스트

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

## comment

궁금한 사항이나 퀴즈 풀이 업로드시 댓글을 이용해주세요.


