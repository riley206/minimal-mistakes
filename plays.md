---
layout: single
title: "Plays"
permalink: /plays/
---

{% for play in site.plays %}
- [{{ play.title }}]({{ site.baseurl }}{{ play.url }})
{% endfor %}
