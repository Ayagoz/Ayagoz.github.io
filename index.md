---
layout: default
title: "Home"
---

<div class="home-intro">
  <h1>Welcome to Ayagoz's Blog</h1>
  <p>I'm Ayagoz, a Deep Learning Engineer exploring the world of AI, neuroscience, and more. Here you'll find my latest thoughts, research, and updates.</p>
</div>

<div class="recent-posts">
  <h2>Recent Blog Posts</h2>
  <ul>
    {% for post in site.posts limit:3 %}
      <li>
        <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
        <p>{{ post.excerpt | strip_html | truncate: 160 }}</p>
      </li>
    {% endfor %}
  </ul>
  <a href="/blog/" class="btn">View All Blog Posts</a>
</div> 