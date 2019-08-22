---
layout: default
redirect_from: "./"
namespace: about
permalink: /about-us/
permalink_de: /ueber-uns/
---

<ul class="post-list">
    {% assign posts=site.posts | where:"lang", page.lang %}
    {% for post in posts %}
      <li>
        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
      </li>
    {% endfor %}
</ul>


[back](./)
