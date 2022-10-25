---
layout: post
title: My Songs
description: Some covered songs I recorded
---
I love singing during rest. Here are some recordings I covered.

<div class="ProjectContainer">
    <div class="gallery">
        {% for item in site.data.showcase %}
        {% if item.domain == "songs" %}
        <div>
        <h3> {{item.title}} </h3>
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
        {% endif %}
        {% endfor %}
      
    </div>
</div>