---
layout: default
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
const urlParams = new URLSearchParams(window.location.search);
const myParam = urlParams.get('t');
const url="{{site.data.urls.unitiddler}}#"+myParam
const frame='<iframe  style="border:0px;" height="750" width="100%" src="'+url+'"></iframe>'
window.onload = function() {
  //console.log("LOADING",frame)
   console.log(frame)
   document.getElementById("main").innerHTML=frame;
}

</script>
<div id="main" role="main">
</div>
