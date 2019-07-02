---
layout: page
title: Infra
permalink: /infra/
pagination:
  enabled: true
---

{%- if paginator.posts.size > 0 -%}
  <div class="post-list">
    {%- for post in paginator.posts -%}
      {%- if post.categories contains 'infra' -%}

        {%- include post-list-item.html -%}

      {%- endif -%}
    {%- endfor -%}
  </div>
{%- endif -%}
