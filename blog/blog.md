---
layout: page
title: Blog
permalink: /blog/
pagination:
  enabled: true
---

{%- if paginator.posts.size > 0 -%}
  <div class="post-list">
    {%- for post in paginator.posts -%}
      {%- include post-list-item.html -%}
    {%- endfor -%}
  </div>
{%- endif -%}
