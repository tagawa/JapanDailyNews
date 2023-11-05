---
layout: default
title: "Japanese Proverbs"
summary: Japanese proverbs with English translation and audio pronunciation guide.
permalink: /proverbs
---
<main class="list">
  <p>{{ page.summary }}
  <p>A work in progress…</p>
  
<div class="card-grid">
  
    {% for proverb in site.data.proverbs offset:1 %}
      <div class="cards">
        <h2>
          <a class="post-link" href="{{ proverb.url }}">{{ proverb.title }}</a>
        </h2>
        <p class="meta">{{ proverb.date }}</p>
        <p>{{ proverb.summary }} </p>
      </div>
    {% endfor %}
    
</div>
</main>
