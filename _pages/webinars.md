---
layout: webinars
title: Webinars
permalink: /webinars/
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
     <!--    <li data-target="#carousel-example-generic" data-slide-to="2"></li> -->
    </ol>
    <div class="carousel-inner">
        <div class="item active">
            <img class="slide-image" src="{{site.baseurl}}/images/webinars/webinar-1.jpg" alt="">
        </div>
        <div class="item">
            <img class="slide-image" src="{{site.baseurl}}/images/webinars/webinar-2.jpg" alt="">
        </div>
        <!-- <div class="item">
            <img class="slide-image" src="{{site.baseurl}}/images/webinars/webinars-1.jpg" alt="">
        </div> -->
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
<nav class="pills pills-webinar list-group list-group-horizontal">
    <li class="upcoming active"><a href="/achive/#self" class="list-group-item">Upcoming</a></li>
</nav>

<div class="masonry-container">
{% assign sp = site.webinars | where: "categories", "upcoming" | reverse  %}
{% for post in sp  %}
<a href="{{site.baseurl}}{{post.url}}">
<div class="item">
<div class="thumbnail">
   {% if post.image %}
        <img src="{{site.baseurl}}/images/webinars/{{post.image}}" alt="{{post.title}}">
   {% else %}
        <img src="{{site.baseurl}}/images/webinars/webinar1.jpg" alt="{{post.title}}">
   {% endif %}
    <div class="caption">
        <h4>{{post.title}}</h4>
        <p>{{post.description | truncate: 160}}</p>
    </div>

</div>
</div>
</a>
{% endfor %}
</div>


