---
layout: default
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
const url="{{site.data.urls.unitiddler}}#"+myParam
const frame='<iframe  style="border:0px;" height="750" width="100%" src="'+url+'"></iframe>'
window.onload = function() {
   document.getElementById("main").innerHTML=frame;
}

</script>
<div id="main" role="main">
</div>
