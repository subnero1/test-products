---
layout: page
title:  Pulse
banner : images/pulse-banner.jpg
---

{% for post in site.posts %}
  <div class='big mod modBlogPost'>
    <div class='images'>
      {% for image in post.images %}
        <div class='image'><img alt="" src="{{site.url}}/{{image}}" /></div>
      {% endfor %}
    </div>
    <div class='content'>
      <p class='info'>
        <span>{{post.date | date: "%B %d, %Y" }}</span>
      </p>
      <h3 style="text-transform: none;"><a href="{{post.url}}">{{post.title}}</a></h3>
      <p>{{post.excerpt}}</p>
      <div class='spacing'></div>
      <a class="button small" href="{{post.url}}">Read more</a>
    </div>
  </div>
{% endfor %}