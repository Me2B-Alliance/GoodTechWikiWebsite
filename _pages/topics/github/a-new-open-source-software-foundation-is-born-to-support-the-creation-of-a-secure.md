---
layout: default
---
<style>
.initial-content {
  padding-left:5%;
  padding-right:25px;
}
</style>

## a new open source software foundation is born to support the creation of a secure

No body provided

{% for term in site.data.metamodel.byTitle['a new open source software foundation is born to support the creation of a secure'].nodes %}
### <a href='/_pages/embed?t={{ term.title }}'>{{ term.title }}</a>

{{ term.description }}
{% endfor %}
