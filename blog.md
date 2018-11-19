---
layout: page
title: Blog
permalink: /blog/
---
Take a look at our awesome blog posts! Here you'll find resources, stories from fellow runners, tips, tricks, and much more.

{% for post in site.categories.blog limit:5 %}
  <article style="margin: 30px 10px 30px 10px;">
    <h2>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h2>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    | {{ post.author }}
    <img style="margin: 10px 0px 10px 0px;" src="{{ post.image }}">
    {{ post.intro }} . . .
  </article>
{% endfor %}

<ul>
  {% for blog in site.categoriesMain %}
    <li>
      <a href="">{{ blog.categoriesMain }}</a>
    </li>
  {% endfor %}
</ul>
