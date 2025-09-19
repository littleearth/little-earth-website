---
layout: page
title: Blog
permalink: /blog/
---

# Blog

All posts from Little Earth Solutions:

{%- for post in site.posts -%}
## [{{ post.title }}]({{ post.url | relative_url }})

**{{ post.date | date: "%B %d, %Y" }}** • Posted in: {{ post.categories | join: ", " }}

{{ post.excerpt | default: post.content | strip_html | truncate: 200 }}

[Continue Reading →]({{ post.url | relative_url }})

---

{%- endfor -%}
