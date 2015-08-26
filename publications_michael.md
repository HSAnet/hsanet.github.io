---
layout: page
title: Publications - Michael Faath 
permalink: /pubs_michael/
--- 

## Conferences and Workshops

<ul>
{% for paper in site.data.publications_michael %}
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

## Standards Contributions
<!--
### RFCs
<ul>
{% for standard in site.data.publications_michael %}
  {% if standard.type == 'rfc' %}
  
  <li>
  {% for author in standard.authors %}
    {{ author.name }},
  {% endfor %}

  "{{ standard.title }}",
  <a href="{{ standard.link }}">{{ standard.rfc }}</a>
  </li>
 
  {% endif %}
{% endfor %}
</ul>
-->

### Active
<ul>
{% for standard in site.data.publications_michael %}
  {% if standard.type == 'id-active' %}
  
  <li>
  {% for author in standard.authors %}
    {{ author.name }},
  {% endfor %}

  "{{ standard.title }}",
  <a href="{{ standard.link }}">{{ standard.ref }}</a>, work in progress
  </li>
 
  {% endif %}
{% endfor %}
</ul>

<!--
### Unmaintained
<ul>
{% for standard in site.data.publications_michael %}
  {% if standard.type == 'id-inactive' %}
  
  <li>
  {% for author in standard.authors %}
    {{ author.name }},
  {% endfor %}

  "{{ standard.title }}",
  <a href="{{ standard.link }}">{{ standard.ref }}</a>, work in progress
  </li>
 
  {% endif %}
{% endfor %}
</ul>
-->

<!--
## Other

### Journal Articles
<ul>
{% for article in site.data.publications_michael %}
  {% if article.type == 'journal' %}
  
  <li>
  {% for author in article.authors %}
    {{ author.name }},
  {% endfor %}

  "{{ article.title }}",
  {{ article.journal }},
  {{ article.date }}
  </li>
 
  {% endif %}
{% endfor %}
</ul>
-->

<!--
### Magazine Articles
<ul>
{% for article in site.data.publications_michael %}
  {% if article.type == 'mag' %}
  
  <li>
  {% for author in article.authors %}
    {{ author.name }},
  {% endfor %}

  "{{ article.title }}",
  {{ article.mag }},
  {{ article.date }}
  </li>
 
  {% endif %}
{% endfor %}
</ul>
-->

<!--

### Technical Reports
<ul>
{% for tr in site.data.publications_michael %}
  {% if tr.type == 'tr' %}
  
  <li>
  {% for author in tr.authors %}
    {{ author.name }},
  {% endfor %}

  "{{ tr.title }}",
  {{ tr.tr }},
  {{ tr.date }}
  </li>
 
  {% endif %}
{% endfor %}
</ul>


### Books Chapters
<ul>
{% for chapter in site.data.publications_michael %}
  {% if chapter.type == 'book-ch' %}
  
  <li>
  {% for author in chapter.authors %}
    {{ author.name }},
  {% endfor %}

  "{{ chapter.title }}",
  {{ chapter.book }},
  {{ chapter.date }}
  </li>
 
  {% endif %}
{% endfor %}
</ul>

### Interviews/various
<ul>
{% for interview in site.data.publications_michael %}
  {% if interview.type == 'interview' %}
  
  <li> 
  Interview by
  {% for author in interview.authors %}
    {{ author.name }},
  {% endfor %}

  "{{ interview.title }}",
  {{ interview.source }},
  {{ interview.date }}
  </li>
 
  {% endif %}
{% endfor %}
</ul>

-->

