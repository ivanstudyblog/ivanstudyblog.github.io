---
layout: page
permalink: /projects/
title: Projects
---

<div id="archives">
{% for category in site.categories %}
  <div class="archive-group">
    {% capture category_name %}{{ category | first }}{% endcapture %}
    {% if category_name=='HTML' %}
    <div id="#{{ category_name | slugize }}"></div>
    <p></p>
    <a name="{{ category_name | slugize }}"></a>
    {% for post in site.categories[category_name] %}
    <article class="archive-item">
      <h3><a href="{{ site.baseurl }}{{ post.url }}">{% if post.title and post.title != "" %}{{post.title}}{% else %}{{post.excerpt |strip_html}}{%endif%}</a></h3>
    </article>
    {% endfor %}
    {% endif %}
  </div>
{% endfor %}
</div>
