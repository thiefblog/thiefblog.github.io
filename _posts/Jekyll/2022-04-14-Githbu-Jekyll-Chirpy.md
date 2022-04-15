---
title: Github Jekyll Chirpy
tags: github
categories: Jekyll
---
# Use Github Action Deploy Jekyll Project

#### Push _site/ to Github Page

[Chirpy Theme](https://github.com/cotes2020/chirpy-starter "Chirpy Theme")


1. Identify the following three files
	- tools/test.sh
	- tools/deploy.sh
	- .github/workflows/pages-deploy.yml
2. Github Action Linux command
	- bundle lock --add-platform ruby
	- bundle lock --add-platform x86_64-linux
3. tools/test.sh use html-proofer to test
	- bundle add html-proofer
4. change branch to gh-pagest
	- branch to gh-pages
<!--more-->
