---
title: About Us
date: 2016-11-22T05:57:29+00:00
author: Neependra
layout: page
permalink: /about/
---

 <div class="row">
   <div class="col-md-8 col-md-offset-2">
        <span style="color: #007ee6;"><strong>Yuga</strong></span> means <span style="color: #007ee6;"><strong>epoch or era</strong></span> and this is definitely a Cloud era. And <span style="color: #007ee6;"><strong>Guru</strong> </span>means <span style="color: #007ee6;"><strong>Teacher</strong></span>. We provide Training and Consulting on latest technologies like <strong>Docker, Kubernetes,  CI/CD cycle, GO programming</strong>. We are also proficient in delivering trainings on <strong>Advance Linux, System Programming, Linux Kernel, Python, Debugging and Performance Tuning.&#8221;</strong>
    </div>
</div>
<div class="pb-50"></div>


<div class="about-us">    
    <div class="row">
        <div class="col-md-12">
            <div class="heading-box">
                <h2>Our Team</h2>

                </div>
        </div>
        {% for item in site.data.data.about %}
        <div class="col-md-4">
            <div class="icon-box-1 border-blue">
                <div class="icon">
                    <img style="display: inline-block;" width="80" class="img-circle" src="{{site.baseurl}}{{item.image}}" alt="{{item.name}}">
                </div>
                <h4>{{item.name}}</h4>
                <p class="title"><small>{{item.title}}</small></p>
                   <ul class="social about-social-links inline-block">
                   {% if item.facebook %}
                    <li><a href="{{item.facebook}}"><i class="ion-social-facebook"></i></a></li>
                   {% endif %}
                   {% if item.twitter %}
                    <li><a href="{{item.twitter}}"><i class="ion-social-twitter"></i></a></li>
                    {% endif %}
                    {% if item.linkedin %}
                    <li><a href="{{item.linkedin}}"><i class="ion-social-linkedin"></i></a></li>
                    {% endif %}
                    {% if item.github %}
                    <li><a href="{{item.github}}"><i class="ion-social-github"></i></a></li>
                    {% endif %}
                    {% if item.website %}
                    <li><a href="{{item.website}}"><i class="ion-android-globe"></i></a></li>
                    {% endif %}

                </ul>
            </div>
        </div>
        {% endfor %}
        

    </div>
</div>


<div class="container-fluid pt-80">
<div class="col-md-12">
    <div class="heading-box">
        <h2>Contact Us</h2>
    </div>
</div>

<div class="typeform-widget" data-url="https://cloudyuga.typeform.com/to/pUY7fb" style=" height: 400px; margin-bottom: 100px" > </div> <script> (function() { var qs,js,q,s,d=document, gi=d.getElementById, ce=d.createElement, gt=d.getElementsByTagName, id="typef_orm", b="https://embed.typeform.com/"; if(!gi.call(d,id)) { js=ce.call(d,"script"); js.id=id; js.src=b+"embed.js"; q=gt.call(d,"script")[0]; q.parentNode.insertBefore(js,q) } })() </script> <div style="font-family: Sans-Serif;font-size: 12px;color: #999;opacity: 0.5; padding-top: 5px;" ></div>

<div class="container-fluid pt-80">
<div class="row">
    <div class="col-md-6">
       <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d687.4775030809581!2d77.59076991349004!3d12.910290222055757!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3bae1511fe717de1%3A0x8a45569b1804a6d0!2zMTLCsDU0JzM3LjUiTiA3N8KwMzUnMjcuMyJF!5e0!3m2!1sen!2sin!4v1534244258361" class="map" frameborder="0" allowfullscreen></iframe>
    </div>
    <div class="col-md-6">
        <h4 class=""><b>Cloud Yuga</b></h4>
        <p class=""><small>#1746, 9th Cross Road <br> Marenahalli <br>2nd Phase, JP Nagar <br> Bengaluru, Karnataka</small></p>
    </div>
</div>
</div>