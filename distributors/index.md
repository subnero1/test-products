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
{% assign distributor_pages = site.pages | where:"categories","distributors" %}
<div class='full'>
  <div class='row'>
    <h1 class="thin">{{page.title}}</h1>
    <div><img alt="" src="{{site.baseurl}}/{{page.image}}" usemap="#distributor-map"/></div>
    <map name="distributor-map">
    {% for page in distributor_pages %}
    <area shape='circle' coords="{{ page.coords}}" href="{{page.web}}" target="_blank" alt="{{page.title}}"/>
    {% endfor %}
    </map>
    <p>We have distributors around the world to help you get our products & support locally. See the list of our distributors and their contact information below.</p>
    <div>
      <p>Let us know if you would like to become our distributor.</p>
      <a href='mailto:sales@subnero.com'><button>Become our distributor</button></a>
    </div>
    <div class='four spacing'></div>
    <div class='large-12 columns' class='container'>
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
            {% if page.phone %}            
            <p><i class="fa fa-phone"></i>  
              {% capture phone %}
                {{ page.phone }}
              {% endcapture %}
              {{ phone | lstrip | newline_to_br  }}
            </p>
            {% endif %}
            {% if page.email %}
            <p>
                <i class="fa fa-envelope"></i> 
                <a href='mailto:{{page.email}}'>{{page.email}}</a>
            </p>
            {% endif %}
            {% if page.web %}
            <p><i class="fa fa-globe"></i>
                <a href='{{page.web}}' target="_blank">{{ page.web }}</a>
            </p>
            {% endif %}
            </div>
        </div>
      </div>
    </div>
    </div>
    {% endfor %}
  </div>
</div>
</div>
