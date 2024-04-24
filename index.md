---
layout: col-sidebar
displaytext: OWASP Quebec City
title: OWASP Quebec City
tags: OWASPQC
level: 4
region: North America
country: Canada
meetup-group: quebec-owasp-meetup-group
---

![Quebec City Chapter Logo](assets/images/ville_quebec_981x303.png)

---

# News
{% raw %}
{% assign sorted_news = site.news | sort: 'date' | reverse %}
{% for item in sorted_news %}
## {{ item.title }}
{{ item.content }}
---
{% endfor %}
{% endraw %}

# Events
{% raw %}
{% assign sorted_events = site.events | sort: 'date' | reverse %}
{% for event in sorted_events %}
## {{ event.title }}
**Speaker:** {{ event.speaker }}

{{ event.content }}
---
{% endfor %}
{% endraw %}
