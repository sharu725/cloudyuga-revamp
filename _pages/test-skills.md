---
title: Test Your Skills
author: Neependra
layout: skills
permalink: /test-skills/
---

<div class="job-app">
<div class="job-app-image" style="background-image: url({{site.baseurl}}/images/test-skills.jpg)"></div>
</div>

<div class="pt-80">
<div class="masonry-container">
{% for post in site.posts %}
<a href="{{site.baseurl}}{{post.url}}">
<div class="item">
<div class="thumbnail">
            <img src="{{site.baseurl}}/images/blogs/{{post.image}}" alt="{{post.title}}">
    <div class="caption">
        <h4>{{post.title}}</h4>
        <p><small>{{post.date | date: '%b %d, %Y'}}</small></p>
        {% if post.description %}
        <p>{{post.description | truncate: 160}}</p>
        {% else %}
        <p>{{post.excerpt | strip_html | strip_newlines | truncate: 160}}</p>
        {% endif %}
    </div>
</div>
</div>
</a>
{% endfor %}
</div>
</div>