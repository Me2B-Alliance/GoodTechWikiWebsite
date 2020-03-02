---
layout: default
---
<style>
.initial-content {
  padding-left:5%;
  padding-right:25px;
}
iframe {
  background: url('/loader.jpg') no-repeat center top;
  background-size: 150px 150px;
  min-height: 350px;
}
</style>

## <a href='/_pages/embed?t=who controls the public sphere in an era of algorithms?'>who controls the public sphere in an era of algorithms?</a>

<iframe style='border:0px;background=white;' width='100%' src='{{site.data.urls.unitiddler}}/#who controls the public sphere in an era of algorithms?'></iframe>

{% for term in site.data.metamodel.byTitle['who controls the public sphere in an era of algorithms?'].nodes %}
### <a href='/_pages/embed?t={{ term.title | url_encode }}'>{{ term.title }}</a>

<a href='{{ term.website | url_encode }}'>{{ term.website }}</a>
<a href='{{ term.url | url_encode }}'>{{ term.url }}</a>

{{ term.description }}
{% endfor %}
