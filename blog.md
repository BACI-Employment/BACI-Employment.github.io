---
layout: page
title: Blog
permalink: /blog/
---
<div class="home wrapper">

  <h1 class="page-heading" style="font-family: 'Open Sans', sans-serif; font-size:35px;">BEST Stories</h1>

  <ul class="post-list" style="font-family: 'Open Sans', sans-serif; ">
    {% for post in site.posts %}
      <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
      </li>
    {% endfor %}
  </ul>

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

</div>