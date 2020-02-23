---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: single
author_profile: false
sidebar:
  nav: sidebar
---
<script>
function doit(e) {
  if(e.value) {
    window.location = e.value  
  }
}
</script>
Who is engaged in
<select onchange="doit(this)">
<option value="">Choose an activity</option>
{% for term in site.data.terms %}<option value="/_pages/embed?t={{term.term}}">{{ term.term }}</option>{% endfor %}</select>

Who is addressing:
<select onchange="doit(this)">
<option value="">Choose a digital harm</option>
{% for term in site.data.harms %}<option value="/_pages/embed?t={{term.term}}">{{ term.term }}</option>{% endfor %}</select>

Record a new
<select onchange="doit(this)">
<option value="">...</option>
<option value="/_pages/inventory/organizations">Organization</option>
<option value="/_pages/inventory/groups">Working Group</option>
<option value="/_pages/inventory/events">Event</option>
<option value="/_pages/inventory/publications">Publication</option>
<option value="/_pages/inventory/product">Product</option>
<option value="/_pages/inventory/product">Service</option>
</select>

<input type="text" id="search" class="search-input" tabindex="-1"
  placeholder="{{ site.data.ui-text[site.locale].search_placeholder_text | default: 'Enter your search term...' }}" />

<div id="results" class="results"></div>
<iframe style="border:0px;" height="750" width="100%" src="{{site.data.urls.mapserver}}#Default"></iframe>
