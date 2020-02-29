---
layout: default
---
<style>
.initial-content {
  padding-left:5%;
  padding-right:25px;
}
</style>

## AI on the Ground (tag)

No body provided

{% for term in site.data.metamodel.byTitle['AI on the Ground (tag)'].nodes %}
### <a href='/_pages/embed?t={{ term.title }}'>{{ term.title }}</a>

{{ term.description }}
{% endfor %}
