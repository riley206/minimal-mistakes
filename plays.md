---
layout: default
title: "Plays"
permalink: /plays/
---

# List of Plays

{% for play in site.plays %}
- [{{ play.title }}]({{ play.url }})
{% endfor %}
