---
layout: page
permalink: /projects/
title: Projects
---


<div id="projects">
{% assign html_category = site.categories.HTML %}
{% if html_category %}
  <div class="archive-group">
    <div id="#html"></div>
    <p></p>
    <h3 class="category-head">HTML</h3>
    <a name="html"></a>
    {% for post in html_category %}
      <article class="archive-item">
        <h4><a href="{{ site.baseurl }}{{ post.url }}">
          {% if post.title and post.title != "" %}
            {{ post.title }}
          {% else %}
            {{ post.excerpt | strip_html }}
          {% endif %}
        </a></h4>
      </article>
    {% endfor %}
  </div>
{% endif %}
</div>
