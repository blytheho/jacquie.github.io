---
layout: page
title: Research
permalink: /research/
position: 2
---

## 2026

<div style="display: flex; flex-direction: column; gap: 1.5rem; margin-bottom: 2.5rem;">
{% for post in site.posts %}
  {% assign post_year = post.date | date: "%Y" %}
  {% if post_year == "2026" %}
  <a href="{{ post.url | relative_url }}" style="text-decoration: none; color: inherit;">
    <div style="display: flex; gap: 1.5rem; align-items: flex-start; flex-wrap: wrap; padding: 1rem; border: 1px solid #e0e0e0; border-radius: 8px; transition: box-shadow 0.2s;">
      {% if post.thumbnail %}
        <img src="{{ post.thumbnail | relative_url }}" alt="{{ post.title }}"
             style="width: 240px; height: 160px; object-fit: cover; border-radius: 6px; flex-shrink: 0;" />
      {% endif %}
      <div style="flex: 1; min-width: 200px;">
        <h3 style="margin-top: 0; margin-bottom: 0.5rem;">{{ post.title }}</h3>
        {% if post.tags.size > 0 %}
          <p style="margin: 0 0 0.5rem; font-size: 0.85em; color: #666;">
            {% for tag in post.tags %}
              <span style="background: #f0f0f0; padding: 2px 8px; border-radius: 4px; margin-right: 4px;">{{ tag }}</span>
            {% endfor %}
          </p>
        {% endif %}
        <p style="margin: 0; color: #555; font-size: 0.95em;">{{ post.excerpt | strip_html | truncate: 200 }}</p>
      </div>
    </div>
  </a>
  {% endif %}
{% endfor %}
</div>

## 2025

<div style="display: flex; flex-direction: column; gap: 1.5rem;">
{% for post in site.posts %}
  {% assign post_year = post.date | date: "%Y" %}
  {% if post_year == "2025" %}
  <a href="{{ post.url | relative_url }}" style="text-decoration: none; color: inherit;">
    <div style="display: flex; gap: 1.5rem; align-items: flex-start; flex-wrap: wrap; padding: 1rem; border: 1px solid #e0e0e0; border-radius: 8px; transition: box-shadow 0.2s;">
      {% if post.thumbnail %}
        <img src="{{ post.thumbnail | relative_url }}" alt="{{ post.title }}"
             style="width: 240px; height: 160px; object-fit: cover; border-radius: 6px; flex-shrink: 0;" />
      {% endif %}
      <div style="flex: 1; min-width: 200px;">
        <h3 style="margin-top: 0; margin-bottom: 0.5rem;">{{ post.title }}</h3>
        {% if post.tags.size > 0 %}
          <p style="margin: 0 0 0.5rem; font-size: 0.85em; color: #666;">
            {% for tag in post.tags %}
              <span style="background: #f0f0f0; padding: 2px 8px; border-radius: 4px; margin-right: 4px;">{{ tag }}</span>
            {% endfor %}
          </p>
        {% endif %}
        <p style="margin: 0; color: #555; font-size: 0.95em;">{{ post.excerpt | strip_html | truncate: 200 }}</p>
      </div>
    </div>
  </a>
  {% endif %}
{% endfor %}
</div>
