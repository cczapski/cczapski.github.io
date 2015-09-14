---
layout: default
title: Blog
permalink: /blog/
---
<div class="post">

  <section class="content">
    <h2 id="Blog">{{page.title}}</h2>
  

    <ul class="blog-container">
      {% for post in site.posts %}
        <li class="blog-content">
          <h2>{{ post.title }}</h2>
          <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
          <p>{{ post.content | truncatewords: 40 }} <a href="{{post.url}}">Read on</a></p>
        </li>
      {% endfor %}
    </ul>

  </section>

</div>

