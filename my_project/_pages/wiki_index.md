// filepath: /workspaces/ser-lo-ma.github.io/my_project/_pages/wiki_index.md
---
layout: default
title: Wiki Index
permalink: /wiki/
---

# Wiki Index

{% for page in site.wiki %}
- [{{ page.title }}]({{ page.url | relative_url }})
{% endfor %}