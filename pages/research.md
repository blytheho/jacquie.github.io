---
layout: page
title: Research
permalink: /research/
position: 2
---

<div>
<h2>2026</h2>
{% for post in site.posts %}{% assign post_year = post.date | date: "%Y" %}{% if post_year == "2026" %}
<a href="{{ post.url | relative_url }}" style="text-decoration: none; color: inherit; display: block;">
<div style="display: flex; gap: 2rem; padding: 1.5rem 0; border-top: 1px solid #e0e0e0;">
  <div style="flex-shrink: 0; min-width: 120px;">
    <p style="margin: 0 0 0.4rem; font-size: 0.85em; color: #888;">{{ post.date | date: "%b %-d, %Y" }}</p>
    {% if post.venue %}<span style="display: inline-block; background: #1a3a4a; color: #fff; font-size: 0.7em; font-weight: 700; padding: 3px 8px; border-radius: 3px; text-transform: uppercase;">{{ post.venue }}</span>{% endif %}
  </div>
  <div style="flex: 1; min-width: 0;">
    <h3 style="margin: 0 0 0.4rem; font-size: 1.15em; line-height: 1.3;">{{ post.title }}</h3>
    {% if post.authors %}<p style="margin: 0 0 0.5rem; font-size: 0.85em; color: #888;">{{ post.authors }}</p>{% endif %}
    <p style="margin: 0; color: #555; font-size: 0.9em; line-height: 1.5;">{{ post.excerpt | strip_html | truncate: 200 }}</p>
  </div>
  {% if post.thumbnail %}<img src="{{ post.thumbnail | relative_url }}" alt="{{ post.title }}" style="width: 200px; height: 130px; object-fit: cover; border-radius: 4px; flex-shrink: 0;" />{% endif %}
</div>
</a>
{% endif %}{% endfor %}

<h2>2025</h2>
{% for post in site.posts %}{% assign post_year = post.date | date: "%Y" %}{% if post_year == "2025" %}
<a href="{{ post.url | relative_url }}" style="text-decoration: none; color: inherit; display: block;">
<div style="display: flex; gap: 2rem; padding: 1.5rem 0; border-top: 1px solid #e0e0e0;">
  <div style="flex-shrink: 0; min-width: 120px;">
    <p style="margin: 0 0 0.4rem; font-size: 0.85em; color: #888;">{{ post.date | date: "%b %-d, %Y" }}</p>
    {% if post.venue %}<span style="display: inline-block; background: #1a3a4a; color: #fff; font-size: 0.7em; font-weight: 700; padding: 3px 8px; border-radius: 3px; text-transform: uppercase;">{{ post.venue }}</span>{% endif %}
  </div>
  <div style="flex: 1; min-width: 0;">
    <h3 style="margin: 0 0 0.4rem; font-size: 1.15em; line-height: 1.3;">{{ post.title }}</h3>
    {% if post.authors %}<p style="margin: 0 0 0.5rem; font-size: 0.85em; color: #888;">{{ post.authors }}</p>{% endif %}
    <p style="margin: 0; color: #555; font-size: 0.9em; line-height: 1.5;">{{ post.excerpt | strip_html | truncate: 200 }}</p>
  </div>
  {% if post.thumbnail %}<img src="{{ post.thumbnail | relative_url }}" alt="{{ post.title }}" style="width: 200px; height: 130px; object-fit: cover; border-radius: 4px; flex-shrink: 0;" />{% endif %}
</div>
</a>
{% endif %}{% endfor %}
</div>
