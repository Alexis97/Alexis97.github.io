---
layout: post
title: My Cover Songs
description: Some songs I've recorded
---
I love singing during rest time. Here are the collection of some songs I've recorded. Hope you like them!

<div >
        {% for item in site.data.showcase %}
        {% if item.domain == "songs" %}
        <div>
        <h3> {{item.title}} </h3>
        {% if item.date %}
            <p class="meta"><small>{{item.date | date: '%B %d, %Y'}}</small></p>
        {% endif %}
        {% if item.intro %}
            <p class="meta"> {{item.intro}} </p>
        {% endif %}
        <p align="center">
        <img src="{{item.image_url}}" alt={{item.name}}/>
        <br>
        <audio
            alt={{item.name}}
            controls
            src="{{item.audio_url}}">
                <a href="{{item.audio_url}}">
                    Download audio
                </a>
        </audio>
        </p>
        </div>
        <br>
        {% endif %}
        {% endfor %}
</div>