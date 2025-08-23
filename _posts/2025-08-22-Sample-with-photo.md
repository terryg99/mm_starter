---
title: "Sample page with image"
excerpt_separator: "<!--more-->"
categories:
  - Blog
tags:
  - Web Development
---

#### This attempts to display sample_image2.png
![sample_image](https://terryg99.github.io/terry-s-first-blog/assets/images/sample_image2.png)

#### This attempts to display sample.png
![sample.png](../sample.png)
{% raw %}{{ site.url }}{{ site.baseurl }}/assets/images/sample_image2.png{% endraw %}

#### This uses a file in same folder
![sample.png](./sample.png)


#### This uses an image source in html 
<img src="./sample.png" />
