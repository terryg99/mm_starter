---
title: "Using Typora to create markdown files"
excerpt_separator: "<!--more-->"
categories:
  - Blog
tags:
  - Web Development
  - Programming
  - Utilities
---

#### TL;DR

Typora is a macOS utility that can be used to create and render markdown files. It "plays nice" with GitHub, allowing the markdown pages to be deployed on the web using GitHub Pages.

#### Introduction

Typora is a macOS app that can be used to generate markdown files. Markdown is a language used to efficiently create plain text files (they can be displayed in TextEdit or BBEdit) that can be rendered into formatted pages. It is a markup language like HTML, but simpler (and only slightly less powerful). The pages in this blog were created as markdown files in Typora, then were uploaded to GitHub, and rendered in GitHub Pages. The technique for doing this is likely to be the subject for future posts in this blog.

Stewart Lynch recommended this app. He mentions it in several of his videos including: [Publish to the web with GitHub Pages and Typora](https://www.youtube.com/watch?v=19Cod5xUV1w) which was the inspiration for this blog.

The utility can be downloaded from: [Typora](https://typora.io). I used the free trial for 15 days then purchased the app for $15 plus tax.

#### What's special about Typora?

There are plenty of markdown editors to choose from. In fact, since markdown files are plain text, they can be created with the TextEdit app which comes free with macOS. So why pay for Typora?

Although we can create a markdown file in TextEdit, we need a way to render it, that is, to interpret the special characters that define formatting and convert the text to the desired style. Most markdown editors can render the plain text as formatted text, but many use a side-by-side approach with the raw text on the left and the rendered text on the right. Typora uses a single pane and displays the rendered text. The markdown characters are only visible when a line is being edited. Personally, I have no problem with the side-by-side approach, or the approach used by GitHub in which the raw text is displayed in one tab and the rendered text in a second tab. But Typora prides themselves on their "distraction free" approach.

Another feature that Typora has is that it provides a sidebar showing the folder/file structure for its markdown files. Linkages to images and other markdown files can be defined by their relative location in this Typora folder hierarchy, then uploaded to the hosting site. If the relative locations are maintained, the links work as expected.

A final feature worth mentioning is that the markdown files created in Typora can be exported as HTML files. If a theme is used to display the rendered markdown in Typora, that special formatting can be translated into HTML and CSS. Initially I used this approach to create styled pages, exported as HTML, then uploaded them to GitHub Pages for deployment. As will be discussed in future posts, I have since moved away from this approach because GitHub Pages can work directly with md files, avoiding the need to convert to HTML.

It's also worth mentioning that there are several "flavors" of markdown. GitHub has a recommended standard called GFM (GitHub Flavored Markdown) and Typora sticks close to that dialect. This makes it easy to upload Typora-generated markdown files to gitHub for deployment via GitHub Pages. More on this in a subsequent post.

