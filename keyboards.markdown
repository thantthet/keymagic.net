---
title: Keyboards
date: 2019-10-20 21:40:00 +06:30
---

<p>Keyboards are now collected in the GitHub repository. You can browse and download the keyboard you want.</p>

<div class="card-grid keyboard-cards">
  {% for keyboard in site.data.keyboards %}
    <a href="https://github.com/thantthet/keymagic-keyboards/raw/refs/heads/master/{{ keyboard.file }}" class="card">
      <i class="card-icon {{ keyboard.icon }}"></i>
      <div class="card-content">
        <h3 class="card-title">{{ keyboard.name }}</h3>
        <h3 class="card-subtitle">{{ keyboard.author }}</h3>
      </div>
    </a>
  {% endfor %}
</div>

## ![keymagic-icon](./assets/icons/keymagic.png) [Keyboard Layout Repository](https://github.com/thantthet/keymagic-keyboards)
