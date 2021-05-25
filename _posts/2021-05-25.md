---
layout: post
title: What is HTML?
subtitle: Excerpt from Soulshaping by Jeff Brown
cover-img: /assets/img/path.jpg
thumbnail-img: /assets/img/thumb.png
share-img: /assets/img/path.jpg
tags: [books, test]
---

HTML is a language that web developers use to add content to, and markup a website – which is why HTML stands for Hyper Text Markup Language. With HTML, we can take human text (the content) - and add markup (special instructions) - to configure that text as something our web browsers can use to display specialized content. Examples of text that have been marked up are ones that display in the form of a list or emphasized.

{% highlight html %}

<ul> </ul>

<em> </em>

{% endhighlight %}

Note: Although some HTML elements will add some styling to the webpage (like the {% highlight html %}<em> {% endhighlight %} tag above), they are not meant to be used for that. Rather, they are meant to provide information to the computer(browser).

Again, HTML is simply what we use to display content on the web, it is no longer a language meant to add style, and it involves no programming concepts – so it is not a programming language.

Basics

You can create HTML content in any text editing application, although you may need a text editor to properly save the file as a HTML file.

The most basic HTML content consists of Tags. HTML Tags define what piece of markup you wish to add to the page and is denounced with angle brackets < >. The browser will read the Tag and define the Markup. The most common Tags are used in pairs and require an (1) opening tag and (2) closing tag i.e.{% highlight html %} <em> </em> {% endhighlight %} The closing Tag requires a forward slash before the Tag name. The other Tags do not require a Closing pair, rather simply the opening and closing angle brackets; some developers like include a forward slash at the end of these tags as a manner of convention (to maintain clean code). There are dozens of HTML Tags available for use, however only some are considered acceptable to use in the most recent version of HTML – HTML5.

Within our Tags we place our Content – which is for the user – as opposed to Tags being for the browser(computer). The Content is simply the text we want to display on the page. For example, {% highlight html %} <em>Hello World</em> {% endhighlight %} where the text ‘Hello World’ is the content. Although Content is mostly focused on the user – it is still important to write in a manner that is easily interpreted by the computer. This is because the computer can be used to dictate that content to the user in multiple ways – such as with screen readers; this combined with properly structured Tags is what we refer to as Semantic HTML.

We can also place content within the HTML angle brackets – after the Tag name – this is referred to as an Attribute. An HTML Attribute is simply a way to provide extra information to the browser, and specifically define what you want to do with your Tag. As stated above – some Tags do not have closing Tags – these tend to rely on their Attribute. An Attribute is written, followed by a colon, and opening and closing quotes to define the attribute content. An example of this is the Image <img> Tag - which will typically include the Source {% highlight html %} <img src: ” ”/> {% endhighlight %} and Alternate {% highlight html %} <img alt: ” ”/> {% endhighlight %}Attributes. The Source Attribute will tell the browser where to access the image you want to use, and the Alternate Attribute will tell the browser what text to display in the event the image does not load.

HTML Tags, Attributes, and Content when combined (or rather completed) are referred to as an HTML Element.

Example of a Basic Document

{% highlight html %}

<!DOCTYPE html>

<html>

<head>

<title>This is a title</title>

</head>

<body>

<!--- This is a Comment --->

<div>

<p>Hello world!</p>

</div>

</body>

</html>

{% endhighlight %}

Required Tags

There are Five required HTML Tags, however the browser will still allow your document to work with Four. The Four Most Important HTML Tags include:

{% highlight html %} <html> {% endhighlight %} The HTML Tag is what defines the start of your document. All other Tags go inside it.

{% highlight html %} <head> {% endhighlight %} The Head Tag is what gives the browser extra information about your document. Inside of it contains Tags such as the Title Tag. This goes within the HTML Tag.{% highlight html %} <html> <head> </head> </html> {% endhighlight %}

{% highlight html %}<title> {% endhighlight %} The Title tag is what appears at the top of your webpage, and it is the main content that is shown on search engine results. This goes within the Head Tag {% highlight html %} <html> <head> <title> <title> </head> </html> {% endhighlight %}

{% highlight html %} <body> {% endhighlight %} The Body Tag contains the content of your document – it is what the user will see on the page. Inside of it contains Tags such as the Paragraph Tag {% highlight html %} <p>{% endhighlight %} This goes within the HTML Tag.{% highlight html %} <html> <body> <body> </html>{% endhighlight %}

Optional, but important still:

{% highlight html %} <!Doctype HTML> {% endhighlight %} This is technically not a Tag, rather it is something that tells the browser what kind of document you are creating, however as of recent most browsers are smart enough to identify that your document is an HTML – so long as all other Tags are correct.

Popular Tags

Besides the ones listed above, as a beginner there are around a dozen or so extremely popular HTML tags; these can be found on almost all websites. They include:

{% highlight html %} <!-- --> {% endhighlight %} The comment tag! Simply put, these are ways for you to leave comments for yourself or others. This is read by the browser, and whatever is in between in it is not display on the webpage for the user.

{% highlight html %} <p> {% endhighlight %} The paragraph tag is used to write normal text and goes within the {% highlight html %} <body> {% endhighlight %}

These are Headings Tags

{% highlight html %} <h1> to <h6> {% endhighlight %} They are used to put headings on your document, and it is particularly important regarding Semantic HTML. These Tags range from H1 to H6(H1, H2, H3, H4, H5, H6), and go from most important to least important (most being H1). It is important to remember that the size and weight of these can be changed later, they are only important for defining importance on your document

These are List Tags

{% highlight html %} <ul> <ol> <li>

{% endhighlight %}Unordered List{% highlight html %} <ul> {% endhighlight %} Ordered List{% highlight html %} <ol> {% endhighlight %} and the List Items{% highlight html %} <li> {% endhighlight %} that go between e.g. {% highlight html %} <ul> <li>List Item</li> <ul>{% endhighlight %} They define lists, Ordered Lists using numbers by default to define order, and Unordered List that uses bullet points by default.

{% highlight html %} <a> {% endhighlight %} This is the Anchor Tag. It is used to define a hyperlink in the document. A hyperlink is simply a way to add a link to a url or directory.

{% highlight html %}<img> {% endhighlight %} This is the Image Tag. It does not have a closing Tag, and it requires Attributes. Particularly one that defines what the image will be and is typically done so by using the Source Attribute{% highlight html %}<img src: ““> {% endhighlight %}

{% highlight html %}<meta> {% endhighlight %} This is the Meta Tag. It is used to define Data within the Head Tag{% highlight html %}<head> {% endhighlight %} Meta Tags (or more commonly referred to as Metadata) always include Attributes. An example of a Meta Tag Attribute would be the Description Attribute; written as {% highlight html %} <meta name=” description” content=” this is what is displayed in your website description”> {% endhighlight %}

{% highlight html %} <div> or <span> {% endhighlight %} The Div and Span Tags do not display anything and are rather placeholders on the document – which is typically manipulated in CSS (Cascading Style Sheets) or JavaScript.

{% highlight html %} <form> {% endhighlight %} The Form Tag is how we create fillable forms on the webpage. The Form Tag simply defines the start of a form and require other Tags to add functionality. Some of those Tags include Input {% highlight html %} <input> {% endhighlight %} Label {% highlight html %} <label> {% endhighlight %} Button {% highlight html %}<button> {% endhighlight %}

{% highlight html %} <script> {% endhighlight %} The Script Tag is how we define the start of JavaScript code, or link to a JavaScript file outside of our document with the Source Attribute {% highlight html %} <script src:””></script>{% endhighlight %} It is not advised to place JavaScript within your document (internal JavaScript) for security reasons.

{% highlight html %}<link> {% endhighlight %} The Link Tag is typically how we Link to external files – particularly CSS (Cascading Style Sheets) which is used to style our document. It is written like this: {% highlight html %}<link rel="stylesheet" href="styles.css"> {% endhighlight %}

{% highlight html %} <button> {% endhighlight %} This is how we define a clickable button on our document. There are also other ways to make buttons, but this is the most common. Buttons are usually attached to links or JavaScript to provide functionality.

Summary

To summarize things: HTML is a Markup Language to define content on our web browsers. HTML consists of Tags, Attributes, and Content – this is what we call an HTML Element.

- Tags define what Markup Element we wish to use.

- Content is what we place between the opening and closing Tags to display on the browser page.

- Attributes add additional information to the Elements.

Some HTML Elements require both an opening and closing Tag, and others do not. The Elements that do not require a Closing Tag will typically require Attributes to further define them.

There are close to if not over a hundred available tags, however there are only a handful that are still relevant in HTML5. This is because of the importance of Semantics (making our document easily readable by the browser), CSS (Cascading Style Sheets) which styles our document, and JavaScript which adds functionality to the website.

Amazing resources to check out for more information are:

[https://www.w3schools.com/tags/default.asp]

[https://developer.mozilla.org/en-US/docs/Web/HTML]

[https://www.toptal.com/designers/htmlarrows/]
