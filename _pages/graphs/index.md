---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: single
sidebar:
  nav: sidebar
---
<style>
.page {
    padding-right:25px;
}
</style>

{% for graph in site.data.graphs %}

# {{ graph.title }}

<a href="/_pages/embedmap?t={{graph.title}}">Open</a>

{{ graph.description }}

{% endfor %}
