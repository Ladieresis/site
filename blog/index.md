---
layout      : default
type        : blog
title       : Blog
permalink   : /blog/
---
<section class="section section--row list-post">
{% for post in site.categories.blog %}
  <article class="list-post__article">
    <a class="list-post__link" href="{{ post.url | prepend: site.baseurl }}">
      <h2 class="list-post__title">
        {{ post.title }}
      </h2>      
      <p class="list-post__description">
        {{ post.description }}
      </p>
    </a>
  </article>
{% endfor %}
</section>
