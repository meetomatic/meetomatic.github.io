---
layout: page
title: "Blog archive"
---

<section class="archive-post-list">

   {% for post in site.posts %}
       {% assign currentDate = post.date | date: "%B %Y" %}
       {% if currentDate != myDate %}
           {% unless forloop.first %}</ul>{% endunless %}
           <h3><a name="{{ post.date | date: "%B-%Y"}}"></a>{{ currentDate }}</h3>
           <ul>
           {% assign myDate = currentDate %}
       {% endif %}
       <li><a href="{{ post.url }}"><span>{{ post.date | date: "%B %-d" }}</span> - {{ post.title }}</a></li>
       {% if forloop.last %}</ul>{% endif %}
   {% endfor %}

</section>