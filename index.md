---
layout: base.liquid
---

# Welcome to my site!

## Create a basic website/ blog-page to rank your site to the top

### Use the power SSG to ship sites in <1s.

{% for post in collections.posts reversed %}
  <a href="{{ post.url }}">
    <h2>{{ post.data.title }}</h2>
    <time>{{ post.data.date | date: "%B %d, %Y" }}</time>
  </a>
{% endfor %}