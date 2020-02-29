---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
---
<style>
.page {
    padding-right:25px;
}
</style>

# Digital Harms Model

Who is addressing:
<select onchange="doit(this)">
<option value="">Choose a digital harm</option>
{% for term in site.data.terms.harms %}<option value="/_pages/embed?t={{term.term}}">{{ term.term }}</option>{% endfor %}</select>

# Activities

Who is engaged in
<select onchange="doit(this)">
<option value="">Choose an activity</option>
{% for term in site.data.terms.activities %}<option value="/_pages/embed?t={{term.term}}">{{ term.term }}</option>{% endfor %}</select>


# Purposes

Who is engaged in
<select onchange="doit(this)">
<option value="">Choose an activity</option>
{% for term in site.data.terms.activities %}<option value="/_pages/embed?t={{term.term}}">{{ term.term }}</option>{% endfor %}</select>


# Tech Focus

Who is engaged in
<select onchange="doit(this)">
<option value="">Choose an activity</option>
{% for term in site.data.terms.activities %}<option value="/_pages/embed?t={{term.term}}">{{ term.term }}</option>{% endfor %}</select>
