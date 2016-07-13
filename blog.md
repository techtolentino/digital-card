---
layout: page
title: it was written
subtitle: A collection of thoughts
---

<h1 class="home--subtitle text--bold">on life,<br>familyhood,<br>& code.</h1>
<hr class="divider--gray">

<ul class="post-list">
    {% for post in site.posts %}
      <li class="post-list-item">
        <h4 class="post-title">
            <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }} ▸</a>
        </h4>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
      </li>
    {% endfor %}
</ul>
