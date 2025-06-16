---
layout: home
title: "Welcome"
permalink: /
show_intro: false
---

## 👋 About Me

Hi, I’m **Steven Lanciotti** — a technical problem-solver passionate about empowering others through code and data. I build tools to simplify complex problems, from data analysis to full-stack applications.  
[More about me →](/about/)

---

## 🚀 Featured Projects

{% assign projects = site.data.homepage.projects %}
<div class="cards">
  {% for p in projects %}
    <a href="{{ p.url }}" class="card">
      <img src="{{ p.image_path }}" alt="{{ p.alt }}">
      <div class="card-content">
        <h3>{{ p.title }}</h3>
        <p>{{ p.excerpt }}</p>
      </div>
    </a>
  {% endfor %}
</div>

<style>
.cards {
  display: grid;
  grid-template-columns: repeat(auto-fill,minmax(250px,1fr));
  gap: 1.5rem;
}
.card {
  background: #fff;
  border-radius: 6px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.1);
  text-decoration: none;
  color: inherit;
  overflow: hidden;
  transition: transform .2s;
}
.card:hover { transform: translateY(-4px); }
.card img { width: 100%; height: 160px; object-fit: cover; }
.card-content { padding: 1rem; }
</style>