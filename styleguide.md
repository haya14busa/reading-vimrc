---
layout: default
title: vimrc style guide
---

vimrc style guide
-----------------

English
=======

Table of Content
----------------
<ul>
{% for guide in site.data.vimrc_style_guide %}
  <li><a href="#{{guide.id}}_en">{{guide.title.en}}</a></li>
{% endfor %}
</ul>

{% for guide in site.data.vimrc_style_guide %}
<h3 id="{{guide.id}}_en">{{ guide.title.en }}</h3>

{{ guide.content.en }}

#### 該当ヘルプ

{% for h in guide.help %}
- {{ h }}
{% endfor %}

{% endfor %}


<hr>

日本語
======

{% for guide in site.data.vimrc_style_guide %}
### {{ guide.title.ja }}

{{ guide.content.ja }}

#### 該当ヘルプ

{% for h in guide.help %}
- {{ h }}
{% endfor %}

{% endfor %}



