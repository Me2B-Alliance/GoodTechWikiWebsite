---
layout: default
---
<style>
.initial-content {
  padding-left:5%;
  padding-right:25px;
}
</style>

## ongoing community drafts

No body provided

{% for term in site.data.metamodel.byTitle['ongoing community drafts'].nodes %}
### <a href='/_pages/embed?t={{ term.title }}'>{{ term.title }}</a>

{{ term.description }}
{% endfor %}
