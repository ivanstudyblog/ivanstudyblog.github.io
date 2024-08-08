---
layout: page
permalink: /categories/
title: Categories
---

<div id="archives">
  {% for category in site.categories %}
    <div class="archive-group">
      {% capture category_name %}{{ category | first }}{% endcapture %}
      <div id="#{{ category_name | slugize }}"></div>
      <p></p>
      
      <!-- Display the category name with the count of posts -->
      <h3 class="category-head">{{ category_name }} ({{ site.categories[category_name].size }})</h3>
      <a name="{{ category_name | slugize }}"></a>
    </div>
  {% endfor %}
</div>
