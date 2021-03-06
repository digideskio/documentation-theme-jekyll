---
title: Syntax highlighting
tags: [formatting]
keywords: rouge, pygments, prettify, color coding,
last_updated: August 12, 2015
summary: "You can apply syntax highlighting to your code. This theme uses pygments and applies color coding based on the lexer you specify."
---


## About syntax highlighting
For syntax highlighting, use fenced code blocks optionally followed by the language syntax you want:

<pre>
```ruby
    def foo
      puts 'foo'
    end
```
</pre>

This looks as follows:

```ruby
    def foo
      puts 'foo'
    end
```

Fenced code blocks require a blank line before and after.

If you're using an HTML file, you can also use the `highlight` command with Liquid markup:

<pre>
{% raw %}{% highlight ruby %}
    def foo
      puts 'foo'
    end
{% endhighlight %}{% endraw %}
</pre>

It renders the same: 

{% highlight ruby %}
    def foo
      puts 'foo'
    end
{% endhighlight %}


The theme has syntax highlighting specified in the configuration file as follows:

```
highlighter: pygments
```

You can use another highlighter such as `rouge`.

The syntax highlighting is done via the css/syntax.css file.

## Available Pygments lexers

The keywords you must add to specify the highlighting (in the previous example, `ruby`) are called "lexers." You can search for "pygments lexers" or go directly to [Available lexers](http://pygments.org/docs/lexers/) to see what values you can use. Here are some common ones I use:

* js
* html
* yaml
* css
* json
* php
* java
* cpp
* dotnet
* xml
* http

