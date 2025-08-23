---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

{% include base_path %}

# Projects

<ul>
  {% for post in site.projects %}
    {% assign num = post.path | split: "-" | last | split: "." | first | plus: 0 %}
    {% if num >= 1 and num <= 6 %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>  
        <p><em>{{ post.excerpt }}</em></p>
      </li>
    {% endif %}
  {% endfor %}
</ul>


