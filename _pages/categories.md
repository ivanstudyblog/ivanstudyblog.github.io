---
layout: page
permalink: /categories/
title: Categories
---

<style>
  /* Styling the dropdown */
  #category-select {
    width: 100%;
    padding: 10px;
    font-size: 16px;
    border: 2px solid #ccc;
    border-radius: 5px;
    background-color: #f9f9f9;
    margin-bottom: 20px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  }

  /* Styling the category content */
  .category-content {
    margin-top: 20px;
    padding: 15px;
    border: 1px solid #e1e1e1;
    border-radius: 5px;
    background-color: #ffffff;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
  }

  /* Styling the category titles */
  .category-head {
    font-size: 22px;
    font-weight: bold;
    margin-bottom: 10px;
    color: #333;
  }

  /* Styling the post titles */
  .archive-item h4 {
    font-size: 18px;
    margin: 5px 0;
    color: #0073e6;
  }

  .archive-item h4 a {
    text-decoration: none;
  }

  .archive-item h4 a:hover {
    text-decoration: underline;
  }

  /* Styling the chart */
  #category-chart-container {
    margin-top: 30px;
    padding: 15px;
    border: 1px solid #e1e1e1;
    border-radius: 5px;
    background-color: #ffffff;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
  }

  #category-chart {
    width: 100%;
    height: 400px;
  }
</style>

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

  <!-- Bar Chart Container -->
  <div id="category-chart-container">
    <canvas id="category-chart"></canvas>
  </div>
</div>

<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
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

  // JavaScript to create the bar chart
  var ctx = document.getElementById('category-chart').getContext('2d');
  var categoryData = {
    labels: [
      {% for category in site.categories %}
        {% capture category_name %}{{ category | first }}{% endcapture %}
        "{{ category_name }}",
      {% endfor %}
    ],
    datasets: [{
      label: 'Number of Posts',
      data: [
        {% for category in site.categories %}
          {{ site.categories[category_name].size }},
        {% endfor %}
      ],
      backgroundColor: 'rgba(0, 123, 255, 0.5)',
      borderColor: 'rgba(0, 123, 255, 1)',
      borderWidth: 1
    }]
  };

  var categoryChart = new Chart(ctx, {
    type: 'bar',
    data: categoryData,
    options: {
      responsive: true,
      scales: {
        y: {
          beginAtZero: true,
          ticks: {
            precision: 0
          }
        }
      }
    }
  });
</script>
