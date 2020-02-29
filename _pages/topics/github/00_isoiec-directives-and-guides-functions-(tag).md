---
layout: default
---
<style>
.initial-content {
  padding-left:5%;
  padding-right:25px;
}
</style>

## 00_ISO/IEC Directives and Guides Functions (tag)

No body provided

{% for term in site.data.metamodel.byTitle['00_ISO/IEC Directives and Guides Functions (tag)'].nodes %}
### <a href='/_pages/embed?t={{ term.title }}'>{{ term.title }}</a>

{{ term.description }}
{% endfor %}
