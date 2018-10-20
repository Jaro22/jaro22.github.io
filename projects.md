---
layout: home
title: "Projects"
weight: 1
---
{%- if site.projects.size > 0 -%}
    {%- for project in site.projects -%}
    <h3>
        <a class="post-link" href="{{ project.url | relative_url }}">
        {{ project.title | escape }}
        </a>
    </h3>
    {%- if site.show_excerpts -%}
        {{ project.description }}
    {%- endif -%}
    {%- endfor -%}
{%- endif -%}