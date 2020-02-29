---
layout: default
---
<style>
.initial-content {
  padding-left:5%;
  padding-right:25px;
}
</style>

## who controls the public sphere in an era of algorithms?

No body provided

{% for term in site.data.metamodel.byTitle['who controls the public sphere in an era of algorithms?'].nodes %}
### <a href='/_pages/embed?t={{ term.title }}'>{{ term.title }}</a>

{{ term.description }}
{% endfor %}
