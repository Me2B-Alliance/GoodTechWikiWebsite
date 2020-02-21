---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: single
author_profile: false
sidebar:
  nav: sidebar
---
I'm looking for information about
<select>{% for term in site.data.terms %}<option>{{ term.term }}</option>{% endfor %}</select>


![image-title-here](/graph1.png){:class="img-responsive"}
