---

title: "Marathons"
permalink: /marathons/
author_profile: true
--------------------

# 🏃🏻 Marathons

|                                           No. | Race                     | Location                | Date                | Time                |
| --------------------------------------------: | ------------------------ | ----------------------- | ------------------- | ------------------- |
| {% assign total = site.data.marathons.size %} |                          |                         |                     |                     |
|     {% for marathon in site.data.marathons %} |                          |                         |                     |                     |
|                      {% assign number = total | minus: forloop.index0 %} |                         |                     |                     |
|                                  {{ number }} | {{ marathon.race }}      | {{ marathon.location }} | {{ marathon.date }} | {{ marathon.time }} |
|                                  {% endfor %} |                          |                         |                     |                     |
