---
title: Test Your Skills
author: Neependra
layout: skills
permalink: /test-skills/
---

<div class="relative">
    <div class="job-app-image" style="background-image: url({{site.baseurl}}/images/test-skills.jpg)"></div>
    <div class="absolute head-text">
    <h1 class="text-center">{{page.title}}</h1>
    </div>
</div>

<div class="pt-80">
<div class="masonry-container">

{% for item in site.data.data.test %}
<a href="{{site.baseurl}}{{item.link}}">
<div class="item">
<div class="thumbnail">
            <img src="{% if item.image %}{{site.baseurl}}/img/{{item.image}}{% else %}{{site.baseurl}}/img/test-your-skills.png{% endif %}" alt="{{item.title}}">
    <div class="caption">
        <h4>{{item.title}}</h4>
        <p>{{item.description}}</p>
    </div>
</div>
</div>
</a>
{% endfor %}
</div>
</div>

