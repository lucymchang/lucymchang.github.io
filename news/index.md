---
title: News
layout: default
---

<!--# {{ page.title }}-->

<div class="twitter-wrapper">
<a class="twitter-timeline" data-width="200" data-height="600" data-theme="light" href="https://twitter.com/lucymchang">Tweets by lucymchang</a> <script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>
</div>

<div id="blog">

{% for post in site.posts %}
<h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
<p><em>{{ post.date | date: "%B %-d, %Y" }}</em></p>
{{ post.content | markdownify }}
<hr/>
{% endfor %}

</div>
