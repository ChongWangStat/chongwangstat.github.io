---
title: "Publications"
permalink: /publications/
author_profile: true
---

# Publications

Peer-reviewed journal articles. An asterisk (*) indicates a Wang student.

<div class="publications-list">
{% for pub in site.data.publications %}
  <p class="publication">
    <strong>{{ forloop.rindex }}.</strong>
    {{ pub.citation | escape }}
    {% if pub.doi_url and pub.doi_url != "" %}
      <a href="{{ pub.doi_url | escape }}" target="_blank" rel="noopener noreferrer">DOI</a>
    {% endif %}
  </p>
{% endfor %}
</div>
