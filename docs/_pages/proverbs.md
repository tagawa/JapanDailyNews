---
layout: default
title: "Japanese Proverbs"
summary: Japanese proverbs with English translation and audio pronunciation guide.
permalink: /proverbs
---
<main class="list">
  <p>{{ page.summary }}</p>
  <p>A work in progress…</p>
  
<div class="card-grid">
  
    {% for proverb in site.data.proverbs %}
      <div class="cards">
        <h2>
          <a class="post-link" href="{{ proverb.url }}">{{ proverb.Proverb }}</a>
        </h2>
        <p class="meta">{{ proverb.Hiragana }}</p>
        <p>{{ proverb.summary }} </p>
      </div>
    {% endfor %}
    
</div>
</main>
