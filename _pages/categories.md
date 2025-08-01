---
layout: page
permalink: /esoc/
title: ESoC skore contributions
---

<h1>My GitHub Contributions to skore</h1>
<ul id="commits"><strong>Commits</strong></ul>
<ul id="prs"><strong>Pull Requests</strong></ul>
<ul id="issues"><strong>Issues</strong></ul>

<script>
const user = 'divakaivan';
const repo = 'probabl-ai/skore';

async function fetchCommits() {
  const url = `https://api.github.com/repos/${repo}/commits?author=${user}`;
  const res = await fetch(url);
  const data = await res.json();
  const container = document.getElementById('commits');
  data.forEach(commit => {
    const li = document.createElement('li');
    li.innerHTML = `<a href="${commit.html_url}" target="_blank">${commit.commit.message}</a>`;
    container.appendChild(li);
  });
}

async function fetchPRs() {
  const url = `https://api.github.com/search/issues?q=repo:${repo}+is:pr+author:${user}`;
  const res = await fetch(url);
  const data = await res.json();
  const container = document.getElementById('prs');
  data.items.forEach(pr => {
    const li = document.createElement('li');
    li.innerHTML = `<a href="${pr.html_url}" target="_blank">${pr.title}</a>`;
    container.appendChild(li);
  });
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

fetchCommits();
fetchPRs();
fetchIssues();
</script>
