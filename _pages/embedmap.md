---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: single
---
<style>
.page {
    padding-right:25px;
}
iframe {
  background: url("/loader.jpg") no-repeat center top;
  background-size: 150px 150px;
  min-height: 650px;
}
</style>
<script>
const urlParams = new URLSearchParams(window.location.search);
const myParam = urlParams.get('t');
const url="{{site.data.urls.mapserver}}#"+myParam
const frame='<iframe style="border:0px;" height="750" width="100%" src="'+url+'"></iframe>'
window.onload = function() {
   document.getElementById("target").innerHTML=frame;
}

</script>
<div id="target">
</div>
