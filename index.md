---
layout: default
title: Home
---

##So, I'm trying out this static site thing

The setup is a *little* unintuitive, but it could be quite cool. For my modest blogging needs, it really could work.

<div id="home">
  <h1>Blog Posts</h1>
  <ul class="posts">
    {% for post in site.posts %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="/teststatic/{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
</div>