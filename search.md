---
layout: default
title: Search
---

# Search

<style>

ol,  ul {  margin: 0; padding: 0; margin-left: 30px;}

.js-search-results { padding-top: 0.2rem; }

.search-results-list-item { padding-bottom: 1rem; }

.search-results-list-item .search-result-title { font-size: 16px; color: #d9230f; }

.search-result-rel-url { color: silver; }

.search-results-list-item a { display: block; color: #777; }

.search-results-list-item a:hover, .search-results-list-item a:focus { text-decoration: none; }

.search-results-list-item a:hover .search-result-title { text-decoration: underline; }

.search-result-rel-date { color: #6d788a; font-size: 14px; }

.search-result-preview { color: #777; font-size: 16px; margin-top: .02rem !important; margin-bottom: .02rem !important; }

.search-result-highlight { color: #2e0137; font-weight: bold; }

.form-control, .form-select {

   min-height: 34px;
   padding: 6px 8px;
   font-size: 16px;
   line-height: 20px;

   vertical-align: middle;
   background-color: #fff;

   border: 1px solid #d1d5da;
   border-radius: 3px;
   
   display: block;
   width: 100%;
}

</style>

<div class="search">
    <div class="search-input-wrap">
    <input type="text" class="js-search-input search-input input-block form-control" tabindex="0" placeholder="Search {{ site.title }}" aria-label="Search {{ site.title }}" autocomplete="off">
    </div>
    <br>
    <div class="js-search-results search-results-wrap"></div>
</div>

<script src="/public/js/lunr.js"></script>
<script src="/public/js/search.js"></script>