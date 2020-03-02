---
layout: default
---
<style>
.initial-content {
  padding-left:5%;
  padding-right:25px;
}
iframe {
  background: url("/loader.jpg") no-repeat center top;
  background-size: 150px 150px;
  min-height: 650px;
}
</style>
<script>
function doit(e) {
  if(e.value) {
    window.location = e.value  
  }
}
</script>


Search for organizations<br />
<input type="text" id="search" class="search-input" tabindex="-1"
  placeholder="{{ site.data.ui-text[site.locale].search_placeholder_text | default: 'Enter your search term...' }}" />

Look for organizations engaged in
<select onchange="doit(this)">
<option value="">Choose an activity</option>
{% for term in site.data.metamodel.types.dimension.activity %}<option value="/_pages/topics/github/{{term[1].page}}">{{ term[1].title }}</option>{% endfor %}</select>


Explore by organization purpose
<select onchange="doit(this)">
<option value="">Choose a purpose</option>
{% for term in site.data.metamodel.types.dimension.purpose %}<option value="/_pages/topics/github/{{term[1].page}}">{{ term[1].title }}</option>{% endfor %}</select>

Explore by concept tag
<select onchange="doit(this)">
<option value="">Choose a tag</option>
{% for term in site.data.metamodel.types.dimension.tag %}<option value="/_pages/topics/github/{{term[1].page}}">{{ term[1].title }}</option>{% endfor %}</select>



<div id="results" class="results"></div>
<iframe style="border:0px;background=white;" height="100%" width="100%" src="{{site.data.urls.mapserver}}?tmap-enlarged=fullscreen&tmap-view=Welcome Graph"></iframe>
