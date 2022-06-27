---
layout: post
title: "在Jekyll博客中使用MathJax"
categories: math
---
{% include math.html %}
1. new file _includes/math.html
```
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
```
2. Use in a markdown or HTML page (or layout) as:
```
\{\% include math.html \%\}
```

3. to test:
  When \(a \ne 0\), there are two solutions to \(ax^2 + bx + c = 0\) and they are
  \[x = {-b \pm \sqrt{b^2-4ac} \over 2a}.\]
