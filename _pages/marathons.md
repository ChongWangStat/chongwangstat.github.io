---
title: "Marathons"
permalink: /marathons/
author_profile: true
---

<table>
  <thead>
    <tr>
      <th>No.</th>
      <th>Race</th>
      <th>Location</th>
      <th>Date</th>
      <th>Time</th>
    </tr>
  </thead>
  <tbody>
    {% for marathon in site.data.marathons %}
      <tr>
        <td>{{ forloop.rindex }}</td>
        <td>{{ marathon.race }}</td>
        <td>{{ marathon.location }}</td>
        <td>{{ marathon.date }}</td>
        <td>
          {% if marathon.result_url and marathon.result_url != "" %}
            <a href="{{ marathon.result_url }}" target="_blank" rel="noopener noreferrer">{{ marathon.time }}</a>
          {% else %}
            {{ marathon.time }}
          {% endif %}
        </td>
      </tr>
    {% endfor %}
  </tbody>
</table>
