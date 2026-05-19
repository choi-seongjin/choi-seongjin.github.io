---
layout: editorial
title: News
editorial_page: News
permalink: "/news/"
---

<section class="page-head">
  <p class="kicker kicker-mark">News</p>
  <h1>The archive.</h1>
  <p class="lede">Reverse chronological. Each item is a permalink; the homepage shows the most recent three. RSS feed at the bottom of the page.</p>
</section>

<section style="padding:20px var(--pad-x) 56px;">

{% assign posts_by_year = site.posts | group_by_exp: "p", "p.date | date: '%Y'" %}
{% for year in posts_by_year %}
  <div style="margin-bottom:36px;">
    <div style="font-family:var(--serif);font-style:italic;font-weight:500;font-size:64px;line-height:1;letter-spacing:-1.5px;color:var(--accent);border-bottom:2px solid var(--ink);padding:8px 0;margin-bottom:16px;">
      {{ year.name }}
    </div>
    {% for post in year.items %}
    <article class="news-entry">
      <div class="date">{{ post.date | date: "%Y·%m·%d" }}</div>
      <div class="tag{% if post.title contains 'Publication' or post.title contains 'TS' or post.title contains 'TR' %} publication{% endif %}">{% if post.subheadline %}{{ post.subheadline }}{% else %}News{% endif %}</div>
      <div>
        <h3>{{ post.title | remove: "[" | remove: "]" | replace: "260112 ", "" | replace: "250307 ", "" | replace: "250420 ", "" | replace: "250424 ", "" | replace: "250425 ", "" | replace: "250225 ", "" | replace: "250107 ", "" | replace: "240903 ", "" | replace: "240901 ", "" | replace: "240621 ", "" }}</h3>
        <p>{{ post.teaser | strip_html | truncate: 320 }}</p>
      </div>
      <div class="arrow">↗</div>
    </article>
    {% endfor %}
  </div>
{% endfor %}

  <div style="margin-top:24px;font-family:var(--mfont);font-size:12px;color:var(--sub);letter-spacing:0.4px;">
    <a href="{{ site.baseurl }}/atom.xml" class="link-underline">Subscribe via RSS ↗</a>
  </div>
</section>
