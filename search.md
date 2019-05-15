---
layout: page
title: Search
---
<!-- Html Elements for Search -->
<div id="search-container">
<input type="text" id="search-input" placeholder="search...">
<ul id="results-container"></ul>
</div>

<!-- Script pointing to search-script.js -->
<script src="/path/to/search-script.js" type="text/javascript"></script>

<!-- Configuration -->
<script>
SimpleJekyllSearch({
  searchInput: document.getElementById('search-input'),
  resultsContainer: document.getElementById('results-container'),
  json: '/search.json'
})
</script>

<div class="search search--dark">
  <div class="main">
    <div class="search__header">{{ _locale_search }}</div>
    <div class="search-bar">
      <div class="search-box js-search-box">
        <div class="search-box__icon-search"><i class="fas fa-search"></i></div>
        <input type="text" />
        <div class="search-box__icon-clear js-icon-clear">
          <a><i class="fas fa-times"></i></a>
        </div>
      </div>
      <button class="button button--theme-dark button--pill search__cancel js-search-toggle">
        {{ _locale_cancel }}</button>
    </div>
    <div class="search-result js-search-result"></div>
  </div>
</div>
<script>{%- include search-providers/default/search.js -%}</script>