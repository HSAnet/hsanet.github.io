---
layout: page
title: Members 
permalink: /members/
menu_order: one
--- 

[Current members](#current) - [Past members](#past)

## <a name="current"></a> Current members

<div>
{% for member in site.data.current_members %}
<div class="profile">
{% if member.photo %} 
    <img src="/img/members/{{ member.photo }}"></img>
{% else %}
    <img src="/img/members/anon.png"></img>
{% endif %}
<h3> {{ member.name }} </h3>
    <b> {{ member.role }}</b>
    <div> {{ member.description }} </div>
    {% if member.pubs %}
    <div><b><a href="/{{ member.pubs }}">Publications</a></b></div>
    {% endif %}
    {% if member.courses %}
    <div><b>Teaching:</b>
    <ul>
    {% for course in member.courses %}
    <li> {{ course.title }} </li>
    {% endfor %}
    </ul></div>
    {% endif %}
</div>
{% endfor %}
</div>

<hr/>

## <a name="past"></a> Past members

<div>
{% for member in site.data.past_members %}
<div class="profile">
{% if member.photo %} 
    <img src="/img/members/{{ member.photo }}"></img>
{% else %}
    <img src="/img/members/anon.png"></img>
{% endif %}
<h3> {{ member.name }} </h3>
    <b> {{ member.role }}</b>
    <div> {{ member.description }} </div>
    {% if member.pubs %}
    <div><b><a href="/{{ member.pubs }}">Publications</a></b></div>
    {% endif %}
</div>
{% endfor %}
</div>