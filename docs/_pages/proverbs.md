---
layout: default
title: "Japanese Proverbs"
summary: Japanese proverbs with English translation and audio pronunciation guide.
permalink: /proverbs
---
<main class="list">
  <p>{{ page.summary }}</p>
  
<div class="card-grid">
  
    {% for proverb in site.data.proverbs %}
      <div class="cards">
        <h2>

        
          {% assign url = "/proverb/" | append: proverb.ID %}
          
          <a class="post-link" href="{{ url }}">{{ proverb.Proverb }}</a>
        </h2>
        <p class="meta">{{ proverb.Hiragana }}</p>
        <p>{{ proverb.EngMeaning }} </p>
      </div>
    {% endfor %}
    
</div>
</main>
