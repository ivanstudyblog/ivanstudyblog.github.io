---
layout: page
permalink: /esoc/
title: ESoC skore contributions
---

<h1>My GitHub Contributions</h1>
<div id="contributions"></div>

<script>
  const url = `https://api.github.com/repos/probabl-ai/skore/commits?author=divakaivan`;

  fetch(url)
    .then(res => res.json())
    .then(data => {
      console.log(data)
    });
</script>
