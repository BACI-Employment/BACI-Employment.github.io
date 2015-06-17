---
layout: page
title: Blog
permalink: /blog/
---

<div style="background-color:#FAFAFA;">
  <div class="container">
        <h1 style="font-family: 'Lobster'; font-size: 100px;">BEST Stories</h1> 
  </div>
</div>

<div class="container">
  <ul class="post-list" style="font-family: 'Open Sans', sans-serif; ">
    {% for post in site.posts %}
      <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </li>
    {% endfor %}
  </ul>

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>
</div>
