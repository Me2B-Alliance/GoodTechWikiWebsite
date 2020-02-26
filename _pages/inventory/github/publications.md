---
layout: single
embed: Publication List
type: publication
sidebar:
  nav: sidebar
---

<style>
.page {
    padding-right:25px;
}
</style>

<ul>
<li><a href="/_pages/inventory/wiki/publications">Wiki</a></li>
<li><a href="{{ site.data.urls.tiddlywiki }}#Publication List">Wiki (external)</a></li>
</ul>

# Table of Contents

<ul>
{% for keys in site.data.nodes.types.publication %}
{% assign subtype = keys[0] %}
  <li>
    <a href="#{{ subtype }}">{{ subtype }}</a>
  </li>
{% endfor %}
</ul>


{% for keys in site.data.nodes.types.publication %}
{% assign subtype = keys[0] %}
# <a name="#{{ subtype }}">{{ subtype }}</a>
<table>
{% for records in keys[1]  %}
{% assign datum = records[1] %}
<tr>
  <td>
    <h2><a href="/_pages/embed?t={{ datum.title }}">{{ datum.title }}</a></h2>
    <div style="width=50%;">{{ datum.description }}</div>
  </td>
  <td>
    <a href="">{{ datum[org.type] }}</a>
  </td>
</tr>

{% endfor %}
</table>
{% endfor %}
