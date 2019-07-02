---
layout: page
title: JavaScript
permalink: /javascript/
pagination:
  enabled: true
---

{%- if paginator.posts.size > 0 -%}
  <div class="post-list">
    {%- for post in paginator.posts -%}
      {%- if post.categories contains 'javascript' -%}

        {%- include post-list-item.html -%}

      {%- endif -%}
    {%- endfor -%}
  </div>
{%- endif -%}
