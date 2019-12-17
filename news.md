---
layout: page
title: News
permalink: /news/
---

<p>News about myMPD and the MPD universe.</p>

<div class="posts">
  {% for post in site.posts %}
    <article class="post">

      <h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>

      <div class="entry">
        {{ post.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a> &ndash; <small>Written on {{ post.date | date: "%B %e, %Y" }}</small>
    </article>
  {% endfor %}
</div>