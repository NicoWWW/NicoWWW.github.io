---
layout: page
title: "Archive"
permalink: /archive/
---


{% for post in site.posts %}
    <div class="row">
        <div class="column column-100">
            <div class="preview-panel">
                <a href="{{ post.url | prepend: site.baseurl }}">
                    <img src="{{ post.preview }}">
                </a>
                <div class="post-title">{{ post.title }}</div>
                <div class="post-summary">{{ post.summary }}</div>
            </div>
        </div>
    </div>
{% endfor %}