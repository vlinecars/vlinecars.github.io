---
layout: default
title: Welcome
exclude: true
---

<div class="home">

  <h1 class="page-heading">Welcome!</h1>
  
  <p>Welcome to <em>V/LineCars.com</em> - the online resource for those interested in the day to day operations, carriages and railcars in service with V/Line - in the present, past and future!</p>
  
  <p><img src="/images/header.jpg" alt="V/Line fleet in the sidings at Southern Cross Station" /></p>
  
  <h2>Recent articles</h2>

  <ul class="post-list">
    {% for post in site.posts offset: 0 limit: 3  %}
      <li>
        <span class="post-meta">{{ post.date | date: "%B %-d, %Y" }}</span>

        <h3>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h3>
		<div class="article-content">
			{{ post.excerpt  | strip_html | truncatewords: 50 }}
		</div>
      </li>
    {% endfor %}
  </ul>
  
  <p><a href="{{ "/articles/" | prepend: site.baseurl }}">More articles</a></p>

  <p class="rss-subscribe">Subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

</div>
