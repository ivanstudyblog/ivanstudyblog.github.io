---
layout: page
permalink: /esoc/
title: ESoC skore contributions
---

<h1>My GitHub Contributions</h1>
<div id="contributions"></div>

<script>
  const username = "divakaivan"; // replace with your username
  const repo = "probabl-ai/skore"; // or loop over multiple repos
  const url = `https://api.github.com/repos/${username}/${repo}/commits?author=${username}`;

  fetch(url)
    .then(res => res.json())
    .then(data => {
      console.log(data)
    });
</script>
