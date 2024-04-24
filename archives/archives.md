---
layout: col-sidebar
title: Archives
---

# News Archive
{% raw %}
{% assign sorted_news = site.news | sort: 'date' | reverse %}
{% for item in sorted_news %}
## {{ item.title }}
{{ item.content }}
---
{% endfor %}
{% endraw %}

# Events Archive
{% raw %}
{% assign sorted_events = site.events | sort: 'date' | reverse %}
{% for event in sorted_events %}
## {{ event.title }}
**Speaker:** {{ event.speaker }}

{{ event.content }}
---
{% endfor %}
{% endraw %}
