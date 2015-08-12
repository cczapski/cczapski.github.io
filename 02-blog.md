---
layout: default
title: Blog
permalink: /blog/
---
<div class="post">

  <section class="content">
    <h2 id="blog">{{page.title}}</h2>
  

    <ul >
      {% for post in site.posts %}
        <li class="blog-content">
          <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

          <h2>
            <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
          </h2>
          <p>{{ post.content | truncatewords: 50 }} <a href="{{post.url}}">Read on</a></p>
        </li>
      {% endfor %}
    </ul>

  </section>

</div>

