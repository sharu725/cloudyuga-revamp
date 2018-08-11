---
title: Jobs
author: Neependra
layout: jobs
permalink: /jobs/
---

<div class="job-app">
<div class="job-app-image" style="background-image: url({{site.baseurl}}/images/job-application.jpg)"></div>
</div>

<br>

<div class="instr archive plain-links">  
<div class="masonry-container">
    {% assign sp = site.jobs | reverse  %}
    {% for post in sp %}
       <a class="" href="{{site.baseurl}}{{post.url}}">
        <div class="item">
            <div class="thumbnail">
                <div class="caption">
                    <h4 class="job-title">{{post.title}}</h4>
                    <hr>
                    <p>{{post.short-desc}}</p>
                    <p>{{post.description | truncate: 160}}</p>
                    <hr>
                    <div class="text-center apply" ><strong>Apply</strong></div>
                </div>
                
            </div>
        </div>
        </a>
    {% endfor %}
    </div>  
    </div>