---
layout: post
title: Inline vs Block Level HTML
subtitle: How HTML Elements Work
cover-img: /assets/img/path.jpg
thumbnail-img: /assets/img/html.png
share-img: /assets/img/path.jpg
tags: [html, development, web]
---

Once you understand what HTML is, the next step is to learn how HTML elements behave in the browser. This is commonly referred to as their default display value. The display value can be one of two things depending on what type of element you are using. They are: 1) Block level, and 2) Inline level.

Block level elements always start on a new line – moving horizontally. Block Level Elements always take up the full width available (as far left and right as possible), and they have a top and bottom margin. Inline elements continue the same line – typically vertically – whilst only taking up as much width as necessary. Of course, however, with CSS we can modify these characteristics – which makes it not as important as we advance.

Some examples of Block level include:

{% highlight html %}

<article>	<figcaption>	<aside>		<figure> 	<div>	<blockquote>	<footer>

<header>	<hr>	<ol>	<li>	<ul>	<main>	<nav>

{% endhighlight %}

![image-title-here](/assets/img/block-level.png){:class="img-responsive"}

Some examples of Inline Elements include:

{% highlight html %}

<a> <br> <button> <em> <img> <input> <label> <script> <span>

{% endhighlight %}

![image-title-here](/assets/img/inline-element.png){:class="img-responsive"}

With HTML5, this concept is now referred to as Phrasing Content, and Flow Content. Phrasing Content, simply put, can be defined as anything that can be placed inside a sentence. These elements can include images, links or emphasized text. Flow Content would be the opposite of Phrasing Content; these are elements that define the sentence, or the run of the sentence – headings, paragraphs, tables etc.
