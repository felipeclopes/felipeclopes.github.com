---
layout: page
title: Content
tagline: Supporting tagline
---
{% include JB/setup %}
    
I pretend to be bloggin often about Rails, Startups and anything that comes to my mind.

## Posts

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

## To-Do

I'm using Jekyll Bootstrap to blog, If you'd like to be added as a contributor, [please fork](http://github.com/plusjade/jekyll-bootstrap)!
There are a lot of things to do, like clean up the themes, make theme usage guides with theme-specific markup examples.