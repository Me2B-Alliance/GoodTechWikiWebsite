---
layout: default
---
<style>
.initial-content {
  padding-left:5%;
  padding-right:25px;
}
</style>

## <a href='/_pages/embed?t=translation dictionary'>translation dictionary</a>

No body provided








{% for term in site.data.metamodel.byTitle['translation dictionary'].nodes %}
### <a href='/_pages/embed?t={{ term.title }}'>{{ term.title }}</a>

<a href='{{ term.website }}'>{{ term.website }}</a>

{{ term.description }}
{% endfor %}
