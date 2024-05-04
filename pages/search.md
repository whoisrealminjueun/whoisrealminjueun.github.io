---
title: search
layout: page
permalink: /search
---

{% assign posts = site.posts | where:"type", "docs" %}

<style>
#search-input {
  box-shadow: none;       /* 그림자 제거 */
  border: none;           /* 외곽선 제거 */
  background-color: transparent;   /* 배경색 제거 */
  caret-color: white;     /* 커서 색상 설정 */
  font-size: 16px;        /* 검색 바 텍스트 크기 조절 */
  color: white;           /* 검색창 텍스트 색상 설정 */
}

#search-input::placeholder {
  font-size: 16px;        /* 검색 바의 임시 텍스트 크기 조절 */
  color: grey;           /* 임시 텍스트 색상 설정 */
}

#search-input:focus {
  outline: none;          /* 포커스 시 외곽선 제거 */
}

#results-container {
  font-size: 16px;        /* 검색 결과 크기 조절 */
  color: white;           /* 검색 결과 텍스트 색상 설정 */
  list-style: none;       /* 검색 결과 목록의 dot 제거 */
  margin-top: 10px;       /* 검색 결과 상단 여백 조절 */
  padding: 0;             /* 검색 결과 내부 여백 제거 */
}

#results-container li {
  margin-bottom: 8px;     /* 검색 결과 간의 행간 조절 */
}
</style>

<p style="display:inline;">Search the <a href="/" style="text-decoration: none; color: blue;">POSTS</a>...</p>
&nbsp;
<!-- Html Elements for Search -->
<div id="search-container">
  <input type="text" id="search-input" placeholder="search...">
  <ul id="results-container"></ul>
</div>

<!-- Script pointing to search-script.js -->
<script src="assets/script/search-script.js" type="text/javascript"></script>

<!-- Configuration -->
<script>
SimpleJekyllSearch({
  searchInput: document.getElementById('search-input'),
  resultsContainer: document.getElementById('results-container'),
  json: '/search.json'
})
</script>
&nbsp;
