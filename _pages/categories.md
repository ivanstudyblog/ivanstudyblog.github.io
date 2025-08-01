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
      const container = document.getElementById("contributions");
      data.forEach(commit => {
        const item = document.createElement("div");
        item.innerHTML = `
          <p><strong>${commit.commit.message}</strong></p>
          <p><a href="${commit.html_url}" target="_blank">View Commit</a></p>
        `;
        container.appendChild(item);
      });
    });
</script>
