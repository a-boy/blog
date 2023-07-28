---
layout: post
title: "在Jekyll博客中使用MathJax"
categories: math
mathjax: true
---

1. new file _includes/math.html
```
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://unpkg.com/mathjax@3/es5/tex-mml-chtml.js"></script>
```
1. Use in a markdown or HTML page (or layout) as:
```
\{\% include math.html \%\}
```
remove 4 \\

or set `mathjax: true` in the *_config.yml* or the markdown’s front matter to **enable** it.

1. to test:
>   When $a \ne 0$, there are two solutions to $$ax^2 + bx + c = 0$$ and   they are
     \\[x = {-b \pm \sqrt{b^2-4ac} \over 2a}.\\]
