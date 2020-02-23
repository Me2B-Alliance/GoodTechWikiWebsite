---
layout: default
---
<script>
const urlParams = new URLSearchParams(window.location.search);
const myParam = urlParams.get('t');
const url="{{site.data.urls.unitiddler}}#"+myParam
const frame='<iframe  style="border:0px;" height="750" width="100%" src="'+url+'"></iframe>'
window.onload = function() {
   console.log(frame)
   document.getElementById("main").innerHTML=frame;
}

</script>
<div id="main" role="main">
</div>
