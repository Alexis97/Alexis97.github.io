---
layout: post
title: 洞箫 (Dong Xiao)
description: Dong Xiao, a.k.a Chinese Phoenix Flute
---
洞箫 (Dong Xiao) is a Chinese traditional musical instrument, a.k.a Chinese Phoenix Flute. I learned how to play Dong Xiao in the Summer of 2021 under [罗守诚 (LUO Shou Cheng)](https://baike.baidu.com/item/%E7%BD%97%E5%AE%88%E8%AF%9A/9894928). [Link to one of Master's work on youtube](https://www.youtube.com/watch?v=wI69SPSCruU).

![Dong Xiao](/assets/images/dongxiao.png)

## My Practice

<div >
        {% for item in site.data.showcase %}
        {% if item.domain == "dongxiao" %}
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



