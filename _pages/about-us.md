---
title: About Us
date: 2016-11-22T05:57:29+00:00
author: Neependra
layout: page
permalink: /about/
---


<span style="color: #00ccff;"><strong>Yuga</strong></span> means <span style="color: #00ccff;"><strong>epoch or era</strong></span> and this is definitely a Cloud era. And <span style="color: #00ccff;"><strong>Guru</strong> </span>means <span style="color: #00ccff;"><strong>Teacher</strong></span>. We provide Training and Consulting on latest technologies like <strong>Docker, Kubernetes,  CI/CD cycle, GO programming</strong>. We are also proficient in delivering trainings on <strong>Advance Linux, System Programming, Linux Kernel, Python, Debugging and Performance Tuning.&#8221;</strong>

<div class="pb-50"></div>

<!-- <div class="row text-center pb-80">
    <div class="col-md-12"><h2>Our Team</h2></div>
    <div class="col-md-6">
        <h3>Neependra Khare</h3>
        <p>Founder and Principal Consultant</p>
        <img style="display: inline-block;" width="100" class="img-circle" src="{{site.baseurl}}/img/neependra-khare.png" alt="Neependra Khare">
    </div>
    <div class="col-md-6">
         <h3>Shiju Varghese</h3>
         <p>Principal Consultant</p>
         <img style="display: inline-block;" width="100" class="img-circle" src="{{site.baseurl}}/img/Shiju-Varghese.png" alt="Shiju Varghese">
    </div>
</div> -->

<div class="about-us">    
    <div class="row">
        <div class="col-md-12">
            <div class="heading-box">
                <h2>Our Team</h2>
                <!-- <p class="sub-heading">A wonderful serenity has taken possession of my entire soul, like these sweet mornings of spring which I enjoy with my whole heart.</p>
                             -->
                </div>
        </div>
        {% for item in site.data.data.about %}
        <div class="col-md-6">
            <div class="icon-box-1">
                <div class="icon">
                    <img style="display: inline-block;" width="100" class="img-circle" src="{{site.baseurl}}{{item.image}}" alt="{{item.name}}">
                </div>
                <h4>{{item.name}}</h4>
                <p class="title"><small>{{item.title}}</small></p>
            </div>
        </div>
        {% endfor %}
        

    </div>
</div>