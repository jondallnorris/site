---
title: projects
layout: page
permalink: /projects
bg_style: graph
---

# Projects

<div class="gallery">
{%- for proj in site.projects -%}
            <figure>
                <a href="{{ proj.url | relative_url }}">
                {%- if proj.img_card -%}
                    <img src="/assets/media/{{proj.img_card}}">
                {% else %}
                    <img src="/assets/media/missing_card.png">
                {%- endif -%}
                </a>
                <figcaption>
                    <h3>{{ proj.title }}</h3>
                    <p> <i>status:</i> {{ proj.status }}</p>
                    <p>{{ proj.description }}</p>
                </figcaption>
            </figure>
{%- endfor -%}

</div>

