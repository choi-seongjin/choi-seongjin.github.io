---
layout: quiet
title: News
permalink: /news/
quiet_active: News
---

<section class="q-page-head">
  <p class="q-eyebrow">News</p>
  <h1>The archive.</h1>
  <p class="q-lede">Reverse chronological. Each item is a permalink; the homepage shows the most recent three.</p>
</section>

<section class="q-section">

{% assign posts_by_year = site.posts | group_by_exp: "p", "p.date | date: '%Y'" %}
{% for year in posts_by_year %}
  <div class="q-year">{{ year.name }}<span class="count">{{ year.items | size }}</span></div>
  {% for post in year.items %}
  <article class="q-news-row">
    <div class="date">{{ post.date | date: "%Y·%m·%d" }}</div>
    <div class="tag">{% if post.subheadline %}{{ post.subheadline }}{% else %}News{% endif %}</div>
    <div>
      <h3>{{ post.title | remove: "[" | remove: "]" | replace: "260112 ", "" | replace: "250307 ", "" | replace: "250420 ", "" | replace: "250424 ", "" | replace: "250425 ", "" | replace: "250225 ", "" | replace: "250107 ", "" | replace: "240903 ", "" | replace: "240901 ", "" | replace: "240621 ", "" }}</h3>
      <p>{{ post.teaser | strip_html | truncate: 200 }}</p>
    </div>
  </article>
  {% endfor %}
{% endfor %}

  <div style="margin-top:32px;font-size:13px;color:var(--sub);letter-spacing:0.4px;">
    <a href="{{ site.baseurl }}/atom.xml" style="color:var(--accent);font-weight:600;">Subscribe via RSS ↗</a>
  </div>

</section>
