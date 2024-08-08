---
layout: page
permalink: /categories/
title: Categories
---

<div id="archives">
  <label for="category-select">Choose a category:</label>
  <select id="category-select" onchange="location = this.value;">
    <option value="">--Select a category--</option>
    {% for category in site.categories %}
      {% capture category_name %}{{ category | first }}{% endcapture %}
      <option value="#{{ category_name | slugize }}">
        {{ category_name }} ({{ site.categories[category_name].size }})
      </option>
    {% endfor %}
  </select>

  <div id="category-list">
    {% for category in site.categories %}
      {% capture category_name %}{{ category | first }}{% endcapture %}
      <div id="{{ category_name | slugize }}" style="display:none;" class="category-content">
        <h3 class="category-head">{{ category_name }} ({{ site.categories[category_name].size }})</h3>
        <a name="{{ category_name | slugize }}"></a>
        {% for post in site.categories[category_name] %}
        <article class="archive-item">
          <h4><a href="{{ site.baseurl }}{{ post.url }}">{% if post.title and post.title != "" %}{{post.title}}{% else %}{{post.excerpt |strip_html}}{%endif%}</a></h4>
        </article>
        {% endfor %}
      </div>
    {% endfor %}
  </div>
</div>

<script>
  // JavaScript to show selected category
  document.getElementById('category-select').addEventListener('change', function() {
    var selectedCategory = this.value;
    var contents = document.querySelectorAll('.category-content');
    contents.forEach(function(content) {
      content.style.display = 'none';
    });
    if (selectedCategory) {
      document.querySelector(selectedCategory).style.display = 'block';
    }
  });
</script>
