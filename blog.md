---
layout: default
title: "Blog"
permalink: /blog/
---

<style>
.blog-heading {
  font-family: 'Playfair Display', serif;
  font-size: 32px;
  font-weight: 600;
  color: #F0EFF8;
  margin-bottom: 0.4rem;
}

.blog-sub {
  font-size: 13.5px;
  color: #6b6a7a;
  margin-bottom: 2.5rem;
  font-family: 'DM Sans', sans-serif;
}

.posts-list {
  list-style: none;
  padding: 0;
}

.post-item {
  background: #1a1a2e;
  border: 1px solid rgba(127,119,221,0.2);
  border-radius: 12px;
  padding: 1.4rem 1.6rem;
  margin-bottom: 14px;
  transition: border-color 0.2s;
}

.post-item:hover {
  border-color: rgba(127,119,221,0.5);
}

.post-item a {
  font-family: 'Playfair Display', serif;
  font-size: 18px;
  font-weight: 500;
  color: #E8E7F5;
  text-decoration: none;
  display: block;
  margin-bottom: 6px;
}

.post-item a:hover { color: #AFA9EC; }

.post-date {
  font-size: 12px;
  color: #3C3A55;
  font-family: 'DM Sans', sans-serif;
  letter-spacing: 0.5px;
}
</style>

<h1 class="blog-heading">Blog Posts</h1>
<p class="blog-sub">Thoughts, learnings, and moments worth remembering.</p>

<ul class="posts-list">
  {% for post in site.posts %}
  <li class="post-item">
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span class="post-date">{{ post.date | date: "%B %d, %Y" }}</span>
  </li>
  {% endfor %}
</ul>
