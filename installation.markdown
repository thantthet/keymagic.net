---
layout: page
title: Installation
description: Step-by-step guides to get KeyMagic running on your preferred operating system.
---

<div class="download-grid">
  {% for platform in site.data.downloads.installation_platforms %}
  <a href="{{ platform.url }}" class="download-card animate delay-{{ forloop.index }}" style="text-decoration: none; min-height: auto; padding: 3rem 2rem;">
    <div class="platform-icon"><i class="{{ platform.icon }}"></i></div>
    <div class="platform-name">{{ platform.name }}</div>
    <div class="btn btn-secondary" style="margin-top: 2rem; width: 100%;">View Guide</div>
  </a>
  {% endfor %}
</div>

<div style="margin-top: 4rem; padding: 2rem; background: var(--surface-color); border: 1px solid var(--surface-border); border-radius: 16px; text-align: center;">
  <p style="color: var(--text-secondary);">
    Need the latest installer? Head over to the <a href="/downloads" style="color: var(--accent-color); text-decoration: none; font-weight: 600;">Downloads</a> page.
  </p>
</div>
