---
layout: page
title: Home
---

# Little Earth Solutions

Welcome to Little Earth Solutions, your source for Delphi development tools and libraries.

## Our Products

* [Backup and Shutdown](/products/backup-and-shutdown/)
* [Signature Wizard](/products/signature-wizard/)
* [delphiXERO](/products/delphixero/)
* [Delphi Library Helper](/products/delphi-library-helper/)
* [NetReflector](/products/netreflector/)
* [LazyREST](/products/lazyrest/)

## Recent Updates

{%- for post in site.posts limit:5 -%}
* [{{ post.title }}]({{ post.url | relative_url }}) - {{ post.date | date: "%B %d, %Y" }}
{%- endfor -%}

[View all posts](/blog/)
