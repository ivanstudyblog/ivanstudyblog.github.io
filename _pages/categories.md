---
layout: page
permalink: /esoc/
title: ESoC skore contributions
---

<h1>My Contributions to <a href="https://github.com/probabl-ai/skore" target="_blank">probabl-ai/skore</a> during my European Summer of Code 2025 stipend period</h1>
<ul id="prs"><strong>Pull Requests</strong></ul>
<ul id="issues"><strong>Issues</strong></ul>

<script>
const user = 'divakaivan';
const repo = 'probabl-ai/skore';

async function fetchPRs() {
  const url = `https://api.github.com/search/issues?q=repo:${repo}+is:pr+author:${user}`;
  const res = await fetch(url);
  const data = await res.json();
  const container = document.getElementById('prs');

  for (const pr of data.items) {
    const prNumber = pr.number;

    // Fetch full PR details to check merged status
    const prDetailsRes = await fetch(`https://api.github.com/repos/${repo}/pulls/${pr.number}`);
    const prDetails = await prDetailsRes.json();

    const isOpen = prDetails.state === 'open';
    const isMerged = prDetails.merged_at !== null;

    if (isOpen || isMerged) {
      const li = document.createElement('li');
      const status = isOpen ? '🟢 Open' : '🟣 Merged';
      li.innerHTML = `<a href="${pr.html_url}" target="_blank">${pr.title}</a> <small>(${status})</small>`;
      container.appendChild(li);
    }
  }
}

async function fetchIssues() {
  const url = `https://api.github.com/search/issues?q=repo:${repo}+is:issue+author:${user}`;
  const res = await fetch(url);
  const data = await res.json();
  const container = document.getElementById('issues');
  data.items.forEach(issue => {
    const li = document.createElement('li');
    li.innerHTML = `<a href="${issue.html_url}" target="_blank">${issue.title}</a>`;
    container.appendChild(li);
  });
}

fetchPRs();
fetchIssues();
</script>
