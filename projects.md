---
layout: home
title: "Projects"
weight: 1
---
{%- if site.projects.size > 0 -%}
    {%- for project in site.projects -%}
    <h3>
        <a class="post-link inline" href="{{ project.url | relative_url }}">
        {{ project.title | escape }}
        </a>
        <small>{{ project.description }}</small>
    </h3>
    {%- endfor -%}
{%- endif -%}