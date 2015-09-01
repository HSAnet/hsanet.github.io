---
layout: page
title: Publications - Fabian Weisshaar 
permalink: /pubs_fabian/
--- 

## Conferences and Workshops

<ul>
{% for paper in site.data.publications_fabian %}
  {% if paper.type == 'conf' %}

    <li>
    {% for author in paper.authors %}
      {{ author.name }},
    {% endfor %} 

    "{{ paper.title }}",
    {{ paper.conf }},
    {{ paper.date }},
    {{ paper.place }}
    </li>

  {% endif %}
{% endfor %}
</ul>

