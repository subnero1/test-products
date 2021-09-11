---
layout: default
title:  Distributors
banner : images/banner-pulse.jpg
image: images/distributors-grey.jpg
---

<div class ='full tall' style='background-image: url({{site.baseurl}}/{{page.banner}});'>
  <div class='row'>
    <div class='large-12 columns'>
    </div>
  </div>
  <div class='four spacing'></div>
  <div class='four spacing'></div>
</div>

<div class='full'>
  <div class='row'>
    <h1 class="thin">{{page.title}}</h1>
    <div><img alt="" src="{{site.baseurl}}/{{page.image}}" /></div>
    <p>We have distributors around the world to help you get our products & support locally. See the list of our distributors and their contact information below.</p>
    <div>
      <p><a href='mailto:sales@subnero.com'>Let us know</a> if you would like to become our distributor.</p>
      <a href='mailto:sales@subnero.com'><button>Become our distributor</button></a>
    </div>
    <div class='four spacing'></div>
    <div class='large-12 columns' class='container'>
    {% assign distributor_pages = site.pages | where:"categories","distributors" %}
    {% for page in distributor_pages %}
    <div class='large-4 columns' id='pulsepage'>
    <div class='mod modBlogPost'>
      <div class='content'>
        <div class='distributor-img'>
        <a target="_blank" href="{{site.baseurl}}{{page.external_url}}">
          <img alt="" src="{{site.baseurl}}/{{page.thumbnail}}" />
        </a>
        </div>
        <div class='distributor-info'>
          <h2>{{ page.title }}</h2>
          {{ page.content }}
        </div>
      </div>
    </div>
    </div>
    {% endfor %}
  </div>
</div>
</div>
