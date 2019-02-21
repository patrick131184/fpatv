---
layout: page
title: Search
image: assets/images/search.jpg
---


<!-- Post Featured Image -->
			{% if page.image %}<img class="featured-image img-fluid" src="{{ site.baseurl }}/{{ page.image }}" alt="{{ page.title }}">{% endif %}
			<!-- End Featured Image -->
      
<!-- Html Elements for Search -->
<div id="search-container">
<input type="text" id="search-input" placeholder="search...">
<ul id="results-container"></ul>
</div>

<!-- Script pointing to search-script.js -->
<script src="{{ site.baseurl }}/assets/js/search-script.js" type="text/javascript"></script>

<!-- Configuration -->
<script>
SimpleJekyllSearch({
  searchInput: document.getElementById('search-input'),
  resultsContainer: document.getElementById('results-container'),
  json: '{{ site.baseurl }}/search.json'
})
</script>
