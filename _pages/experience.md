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
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>  
      <p><em>{{ post.excerpt }}</em></p>
    </li>
  {% endfor %}
</ul>
