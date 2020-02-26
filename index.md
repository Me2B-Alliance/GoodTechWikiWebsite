---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: single
sidebar:
  nav: sidebar
---
<style>
.page {
    padding-right:25px;
}
iframe {
  background: url("/loader.jpg") no-repeat;
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

<p>This is an editable database. Before adding new entries please search for the wiki to see if they are already listed. </p>


<p>
Browse by <a href="/_pages/topics/index">Topics &amp; Tags</a>, such as Digital Harms, Organizational Activities,
or General Semantic tags - or use the search bar below to do a free text search.
</p>


<input type="text" id="search" class="search-input" tabindex="-1"
  placeholder="{{ site.data.ui-text[site.locale].search_placeholder_text | default: 'Enter your search term...' }}" />


Add a new
<select onchange="doit(this)">
<option value="">...</option>
<option value="/_pages/inventory/organizations">Organization</option>
<option value="/_pages/inventory/groups">Working Group</option>
<option value="/_pages/inventory/events">Event</option>
<option value="/_pages/inventory/publications">Publication</option>
<option value="/_pages/inventory/product">Product</option>
<option value="/_pages/inventory/product">Service</option>
</select>

<div id="results" class="results"></div>
<iframe style="border:0px;background=white;" height="100%" width="100%" src="{{site.data.urls.mapserver}}#Welcome Graph"></iframe>
