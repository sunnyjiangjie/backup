---
layout: default
title: Jay Jiang
tagline: a packaging engineer
---
{% include JB/setup %}

<h1>最新文章</h1>

<ul>

<div class="posts">
  {% for post in site.posts %}
    <article class="post">
      <h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>   
	  <div class="date">{{ site.time | date_to_long_string}}</div>
      <div class="entry">
        {{ post.excerpt }}
      </div>

      <strong><a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a></strong>
    </article>
	<br />
	<br />
  {% endfor %}
</div>
</ul>



