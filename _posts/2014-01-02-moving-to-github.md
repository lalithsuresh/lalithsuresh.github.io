---
layout: post
title: ! 'Moving to Github'
type: post
---



It's the New Year and that means it's time for change. I've finally moved my blog off wordpress.com and onto Github + Jekyll.

Jekyll has been a pleasure to deal with so far. The import from wordpress was mostly trivial but with some rough edges.

First, export your wordpress.com blog using the admin console (you should get an xml dump of your site) and then run:

{% highlight bash %}
# Assumes the XML dump is named wordpressdotcom.xml,
$: jekyll import wordpressdotcom
{% endhighlight %}

I only exported my posts because I wanted to setup pages myself. The above command should populate Jekyll's
`_posts` folder with your blog's posts as html files.

I found the generated html to be rather mangled; there were no paragraph separations and blockquotes looked ugly. This required
some monkey patching with `sed` and `awk` to fix. There are still some more loose edges left which I'll get around to later.
I've setup [Disqus](http://disqus.com) for comments, and I still need to import all the comments from the Wordpress site.

I'm currently on the [Hyde theme](http://andhyde.com) which I modified a bit to suit my liking.

All in all, it's been a breeze to deploy over Github and I'm quite happy to have a lot more control on how my site looks like.
