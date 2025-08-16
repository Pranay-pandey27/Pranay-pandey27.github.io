---
layout: archive
title: "Research Experience"
permalink: /experience/
author_profile: true
---

{% include base_path %}

# Experimental Research Experience

<ul>
  {% for post in site.experience %}
    {% assign num = post.path | split: "-" | last | split: "." | first | plus: 0 %}
    {% if num >= 1 and num <= 3 %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>  
        <p><em>{{ post.excerpt }}</em></p>
      </li>
    {% endif %}
  {% endfor %}
</ul>

# Theoretical Research Experience

- **Quantum Machine Learning**

<ul>
  {% for post in site.experience %}
    {% assign num = post.path | split: "-" | last | split: "." | first | plus: 0 %}
    {% if num >= 4 and num <= 6 %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>  
        <p><em>{{ post.excerpt }}</em></p>
      </li>
    {% endif %}
  {% endfor %}
</ul>

- **Quantum Error Correction**

<ul>
  {% for post in site.experience %}
    {% assign num = post.path | split: "-" | last | split: "." | first | plus: 0 %}
    {% if num >= 5 %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>  
        <p><em>{{ post.excerpt }}</em></p>
      </li>
    {% endif %}
  {% endfor %}
</ul>
