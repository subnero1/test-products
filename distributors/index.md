---
layout: default
title:  Distributors
banner : images/banner-pulse.jpg
image: images/Distributors_grey1.jpg
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
    <div class='large-4 columns'>
    <div class='mod modBlogPost'>
      <div class='distributor-cards'>
        <a href='{{page.web}}' target="_blank">
          <div class='distributor-img'>
              <img alt="" src="{{site.baseurl}}/{{page.thumbnail}}" />
          </div>
        </a>
        <div class='distributor-info'>
          <h2>{{ page.title }}</h2>
          <p class='distributor-addr'>{{ page.address }}</p>
          <div class='distributor-info'>
            <p><i class="fa fa-phone"></i>  
              {% capture phone %}
                {{ page.phone }}
              {% endcapture %}
              {{ phone | lstrip | newline_to_br  }}
            </p>
            <p>
                <i class="fa fa-envelope"></i> 
                <a href='mailto:{{page.email}}'>{{page.email}}</a>
            </p>
            <p><i class="fa fa-globe"></i>
                <a href='{{page.web}}' target="_blank">{{ page.web }}</a>
            </p>
            </div>
        </div>
      </div>
    </div>
    </div>
    {% endfor %}
  </div>
</div>
</div>
