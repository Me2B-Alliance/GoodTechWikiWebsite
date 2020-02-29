---
layout: default
---
<style>
.initial-content {
  padding-left:5%;
  padding-right:25px;
}
</style>

## Algorithms and Publics (tag)

No body provided

{% for term in site.data.metamodel.byTitle['Algorithms and Publics (tag)'].nodes %}
### <a href='/_pages/embed?t={{ term.title }}'>{{ term.title }}</a>

{{ term.description }}
{% endfor %}
