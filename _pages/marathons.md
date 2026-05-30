---

title: "Marathons"
permalink: /marathons/
author_profile: true
--------------------

# 🏃🏻 Marathons

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
        <td>{{ marathon.time }}</td>
      </tr>
    {% endfor %}
  </tbody>
</table>
