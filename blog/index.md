---
layout: blog
title: Blog
# video-id: 222773086
# Video-id is the if of the video from Vimeo. Remove the # to see video in place of slider. 
---
 

<div class="col-md-12">
<div class="row carousel-holder">
<div class="col-md-12">
{% if page.video-id %}
        <iframe src="https://player.vimeo.com/video/{{page.video-id}}" class="video-header" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
{% else %}
<div id="carousel-example-generic" class="carousel slide" data-ride="carousel">
    <ol class="carousel-indicators">
        <li data-target="#carousel-example-generic" data-slide-to="0" class="active"></li>
        <li data-target="#carousel-example-generic" data-slide-to="1"></li>
    </ol>
    <div class="carousel-inner">
        <div class="item active">
            <img class="slide-image" src="{{site.baseurl}}/images/blogs/blog-1.jpg" alt="">
        </div>
        <div class="item">
            <img class="slide-image" src="{{site.baseurl}}/images/blogs/blog-2.jpg" alt="">
        </div>
    </div>
<a class="left carousel-control" href="#carousel-example-generic" data-slide="prev">
        <span class="glyphicon glyphicon-chevron-left"></span>
    </a>
    <a class="right carousel-control" href="#carousel-example-generic" data-slide="next">
        <span class="glyphicon glyphicon-chevron-right"></span>
    </a>
</div>
{% endif %}
</div>
</div>
<nav class="pills pills-blog list-group list-group-horizontal">
    <li class="contain active"><a href="/achive/#contain" class="list-group-item">Containers</a></li>
    <li class="community"><a href="/achive/#community" class="list-group-item">Community</a></li>
    <li class="cloudyuga"><a href="/achive/#cloudyuga" class="list-group-item">CloudYuga</a></li>
    <li class="trainings"><a href="/achive/#trainings" class="list-group-item">Trainings</a></li>
</nav>
<div class="contain archive plain-links">                
<div class="masonry-container">
{% assign sp = site.posts | where: "categories", "containers" %}
{% for post in sp %}
<a href="{{site.baseurl}}{{post.url}}">
<div class="item">
<div class="thumbnail">
        {% if post.image %}
            <img src="{{site.baseurl}}/images/blogs/{{post.image}}" alt="{{post.title}}">
        {% else %}
            <img src="{{site.baseurl}}/images/blogs/blog-fallback.jpg" alt="{{post.title}}">
        {% endif %}
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
<div class="community archive plain-links hide">                
<div class="masonry-container">
{% assign sp = site.posts | where: "categories", "community" %}
{% for post in sp %}
<a href="{{site.baseurl}}{{post.url}}">
<div class="item">
<div class="thumbnail">
    {% if post.image %}
        <img src="{{site.baseurl}}/images/blogs/{{post.image}}" alt="{{post.title}}">
    {% else %}
        <img src="{{site.baseurl}}/images/blogs/blog-fallback.jpg" alt="{{post.title}}">
    {% endif %}
    <div class="caption">
        <h4>{{post.title}}</h4>
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
<div class="cloudyuga archive plain-links hide">        
<div class="masonry-container">
{% assign sp = site.posts | where: "categories", "cloudyuga" %}
{% for post in sp %}
<a href="{{site.baseurl}}{{post.url}}">
<div class="item">
<div class="thumbnail">
    {% if post.image %}
        <img src="{{site.baseurl}}/images/blogs/{{post.image}}" alt="{{post.title}}">
    {% else %}
        <img src="{{site.baseurl}}/images/blogs/blog-fallback.jpg" alt="{{post.title}}">
    {% endif %}
    <div class="caption">
        <h4>{{post.title}}</h4>
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
<div class="trainings archive plain-links hide">    
           
<div class="masonry-container">
{% assign sp = site.posts | where: "categories", "trainings" %}
{% for post in sp %}
<a href="{{site.baseurl}}{{post.url}}">
<div class="item">
<div class="thumbnail">
    {% if post.image %}
        <img src="{{site.baseurl}}/images/blogs/{{post.image}}" alt="{{post.title}}">
    {% else %}
        <img src="{{site.baseurl}}/images/blogs/blog-fallback.jpg" alt="{{post.title}}">
    {% endif %}
    <div class="caption">
        <h4>{{post.title}}</h4>
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
<div class="row">
    <div class="col-md-2 text-right pull-right"><a href="/blog/all/">All posts →</a></div>
</div>
</div>


