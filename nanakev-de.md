---
layout: page
title: Nana & Kev
ref: nana-kev
permalink: de/nana-kev
lang: de
---

<ul class="post-list">
    {% assign posts=site.posts | where:"lang", page.lang  | where:"categorie", page.ref %}
    {% for post in posts %}
      <li>

        <h2>
          <a class="post-link" href="{{ post.url}}">{{ post.title }}</a>
        </h2>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
        {{post.content}}

      </li>
    {% endfor %}
  </ul>