---
layout: default
title: Products
banner : images/banner-products.jpg
excerpt: Subnero's underwater acoustic modems with UnetStack for underwater wireless communication and networking and SWAN for real-time water-quality monitoring.
---
<div class='full tall' style='background-image: url({{site.baseurl}}/{{page.banner}});'>
  <div class='row'>
    <div class='large-12 columns'>
      <!-- {% include section-header.html title=page.title tagline=page.tagline color=page.title_color class="big" %} -->
    </div>
  </div>
  <div class='four spacing'></div>
  <div class='four spacing'></div>
</div>

<div class='full'>
  <div class='type-container'>
      <h2>PRODUCT CATEGORY</h2>
  </div>

  <!-- <div class ='category-container '> -->
  {% assign product_pages = site.pages | where:"categories","underwatermodem" %}
  {% for page in product_pages %}
  <div class='category-container bg-grey'>
    <div class='category-img'>
      <img alt="" src="{{site.baseurl}}/images/pulse-thumbnail-ieee-earthzine_grey.jpg"/>
    </div>
    <div class='category-content'>
      <h1>Wireless Networked Communications</h1>
      <h3>Software defined underwater acoustic modems for networking, navigation and monitoring.</h3>
      <div class='media'>
        <div class='modem-type'>
        <p>Low frequency underwater acoustic modems</p>
        <a href='{{site.baseurl}}/products/modem.html'><button>L5L series</button></a>
        </div>
        <div class='modem-type'>
        <p>Medium frequency underwater acoustic modems</p>
        <a href='{{site.baseurl}}/products/modem.html'><button>M25M series</button></a>
        </div>
      </div>
    </div>
  </div>
  {% endfor %}
  {% assign product_pages = site.pages | where:"categories","unet" %}
  {% for page in product_pages %}
  <div class='category-container'>
    <div class='category-img'>
      <img alt="" src="{{site.baseurl}}/images/pulse-thumbnail-ieee-earthzine_grey.jpg"/>
    </div>    
    <div class='category-content'>
      <h1>Underwater Network Stack & Simulator</h1>
      <h3>An agent-based software stack and simulator for underwater networks and protocols.</h3>
      <div class='media'>
        <div class='modem-type'>
        <a href='{{site.baseurl}}/products/unet.html'><button class='unet'>UnetStack Premium</button></a>
        </div>
      </div>
    </div>
  </div>
  {% endfor %}

  {% assign product_pages = site.pages | where:"categories","water-quality-management" %}
  {% for page in product_pages %}
  <div class ='category-container bg-grey'>
    <div class='category-img'>
      <img alt="" src="{{site.baseurl}}/images/pulse-thumbnail-ieee-earthzine_grey.jpg"/> 
    </div>
    <div class='category-content'>
      <h1>Subnero Water Assessment Network</h1>
      <h3>Scalable autonomous platforms for real-time in-situ water quality measurements.</h3>
      <div class='media'>
        <div class='modem-type'>
        <p>SWAN Network and components</p>
        <a href='{{site.baseurl}}/products/swan.html'><button>SWAN</button></a>
        </div>
      </div>
    </div>
  </div>
    {% endfor %}
<!-- </div> -->
<div class='four spacing'></div>
</div>
