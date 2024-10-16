---
layout: default
title: "Plays"
permalink: /plays/
---

# List of Plays

{% for play in site.plays %}
- [{{ play.title }}]({{ site.baseurl }}{{ play.url }})
{% endfor %}
