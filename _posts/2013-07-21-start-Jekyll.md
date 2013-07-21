---
layout: post
styles: [syntax]
title: 开始使用Jekyll在github上搭建博客
---

我以geeklu的模板作为基础，建立了这个个人微博客。

主要的目的是记录一些技术的感悟和体验，以前做过很多事，大多都忘了。涉及的不深，杂而不通。

Web开发几乎不懂，决定开始学一些。这篇主要是尝试各种需要的表示方式。
<pre class="terminal">
  <code>
  $sudo gem install jekyll rdiscount
  $continue...
  $go on...
  </code>
</pre>

一、Jekyll的文件及目录配置：
<pre class="terminal">
  .
  |-- _includes
  |-- _plugins 
  |-- _layout 
  |     |-- default.html
  |     |-- post.html
  |-- _post
  |     |-- yyyy-mm-dd-title.markdown
  |     |-- yyyy-mm-dd-title.markdown
  |-- _site
  |-- _config.yml
  |-- index.html
</pre>

二、目录介绍
## _includes
存放需要在模板中包含的文件，可以使用Liquid标签<code>\{&permil; include file.ext &permial;\}</code>来引用相应的文章

## _plugins
可以增加自己的插件

## _layout
存放布局模板

## _post
存放文章列表，文件命名一定要遵循yyyy-mm-dd-teile.html|markdown|textile 规则

## _site
Jekyll自动生成的，可以忽略

## _config.yml
设置经常使用的配置选项

## index.html 和所有的 HTML/Markdown/Textile文件
所有的HTML/Markdown/TextTile 文件都可以包含 YAML 配置，这类文件都会被Jekyll解析。


