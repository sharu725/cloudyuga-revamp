---
layout: skills
permalink: /consulting/
title: Consulting
---


<div class="relative">
    <div class="job-app-image" style="background-image: url({{site.baseurl}}/images/consulting-header.jpg)"></div>
    <div class="absolute head-text">
    <h1 class="text-center">{{page.title}}</h1>
    </div>
</div>

<div class="pt-80">
    <div class="masonry-container">
        {% for post in site.consulting %}
        <a href="{{post.url}}">
            <div class="item">
                <div class="thumbnail">
                    <img src="{{site.baseurl}}/images/consulting/consulting.jpg" alt="{{post.title}}">
                    <div class="caption">
                    <h4>{{post.title}}</h4>
                    <p>{{post.description | truncate: 160}}</p>
                    </div>
                </div>
            </div>
        </a>
        {% endfor %}
    </div>
</div>



