---
title: Github Jekyll Chirpy
tags: github
---
Use Github Action Deploy Jekyll Project

Push _site/ to Github Page

https://github.com/cotes2020/chirpy-starter

<ol>
  <li>
    Identify the following three files
    <ul>
      <li>tools/test.sh</li>
      <li>tools/deploy.sh</li>
      <li>.github/workflows/pages-deploy.yml</li>
    </ul>
  </li>
  <li>
    Github Action Linux command
    <ul>
      <li>bundle lock --add-platform ruby</li>
      <li>bundle lock --add-platform x86_64-linux</li>
    </ul>
  </li>
  <li>
    tools/test.sh use html-proofer to test
    <ul>
      <li>bundle add html-proofer</li>
    </ul>
  </li>
  <li>
    change branch to gh-pagest
    <ul>
      <li>branch to gh-pages</li>
    </ul>
</li>
</ol>
<!--more-->
