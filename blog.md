---
layout: default
title: "Stories"
permalink: /blog/
description: "Everything published by the Air Quality Life Index blog, newest first, with the exposure each story describes."
---

<main id="main-content" class="page-shell">
  <div class="shell">
    <header class="page-hero">
      <p class="eyebrow">Register</p>
      <h1>Stories</h1>
      <p>Everything published, newest first, with the exposure each story describes.</p>
    </header>

    <div class="page-body">
      {%- if site.posts.size > 0 -%}
      <div class="filter-box filter-box--wide">
        <label for="archive-search">Search stories</label>
        <input id="archive-search" data-post-search type="search" placeholder="Try PM2.5, district, policy, weighting…">
      </div>

      <div class="post-list">
        {%- for post in site.posts -%}
          {% include post-card.html post=post list=true %}
        {%- endfor -%}
      </div>
      <p class="empty-state" data-empty-state hidden>No stories match that search.</p>

      {%- else -%}
      <p class="empty-state">
        The register is empty. When a story is published it will appear here as a dated entry — the
        section it belongs to, the headline, the standfirst, and, for any story about a place, that
        place's position on the exposure ruler, so the register can be read as a scale rather than a
        list.
        <br><br>
        To add the first one: <a class="text-link" href="{{ '/write/' | relative_url }}">the editorial guide</a>,
        then <a class="text-link" href="{{ '/formatting/' | relative_url }}">the formatting reference</a>.
      </p>
      {%- endif -%}
    </div>
  </div>
</main>
