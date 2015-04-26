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
      <h2>{{ post.title }}</h2>   
	  <div class="date">{{ site.time | date_to_long_string}}</div>
      <div class="entry">
        {{ post.excerpt }}
      </div>

      <strong><a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a></strong>
    </article>
	
  {% endfor %}
</div>
</ul>



<ul>
	{% for post in site.posts %}
		<li>{{ site.time | data_to_string }} <h3><a href="{{ site.baseurl }}{{post.url }}">{{post.title}}</a></h3></li>
	{% endfor %}


</ul>
