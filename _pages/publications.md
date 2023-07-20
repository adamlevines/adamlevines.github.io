---
title:  "Publications"
layout: splash
permalink: /publications/
---

<p><h1>Publications</h1></p>

{% assign publications = site.data.publications %}

{% for publication in publications %}
    <h2>{{ publication.year }}</h2>
    <ul>
        <li>
            <b>{{ publication.title }}</b><br>
            {{ publication.authors }}<br>
            <font size="-1"><em>{{ publication.conference }} {{ publication.conference_date }}</em></font><br>
            {% if publication.paper_link %}
                <a href="{{ publication.paper_link }}" style="color: #7393B3;" target="_blank">[paper]</a>
            {% endif %}
        </li>
    </ul>
{% endfor %}
