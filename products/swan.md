---
layout: default
title: Subnero Water Assessment Network
banner : images/banner-SwanBot.jpg
thumbnail: images/boxart-swan.jpg
excerpt: Scalable autonomous platforms for in-situ water quality measurements
categories: water-quality-management
section_id: products
tabs: swancomponents
---

<div class='full tall swan' style='background-image: url({{site.baseurl}}/{{page.banner}});'>
    <div class='large-12 columns'>
      <h2 class='banner-text'>Smart monitoring of the world's most precious resource.</h2>
    </div>
    <div class='large-12 columns'>
        <div class='banner-heading'>
          <h1 class='banner-text'>
            <span class='orange'>S</span>ubnero <span class='orange'>W</span>ater <span class='orange'>A</span>ssessment <span class='orange'>N</span>etwork</h1>
          <h2 class='banner-sub-heading'>Redefine water quality monitoring.</h2>
        </div>
    </div>
</div>
<div class='four spacing'></div>
<div class='row features-row row-padding-bottom'>
    <div class='swan-intro'>
      <p>The Subnero Water Assessment Network (SWAN) is a network of smart surface robots called the SwanBots, that automates the overall process of water quality monitoring. The network provides real-time monitoring and analysis of water quality data along with the ability to collect samples at depth and can span across diverse assets, including SwanBots, sensor nodes, and data analytics systems.</p>
      <p>Let’s take a look at how SWAN solves today’s challenges in water quality monitoring.</p>
      <div class="flex-video video">
        <iframe src="https://www.youtube.com/embed/kNGR6LmSVwE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      </div>
      <a href="mailto:sales@subnero.com" class='centered-text hOXnHC'><button class="button-outline">GET A QUOTE</button></a>
    </div>
</div>
<div class='bg-grey'>
  <div class='row accordion-row'>
    <!-- <div class='large-6 columns'> -->
      <div class='accordion-container bg-white'>
        <div class="accordion-tab">
          <div class="accordion-item">
            <input type="radio" id="rad1" name="radio" hidden>
            <label class="accordion-label" for="rad1">Safe and Sustainable</label>
            <div class="accordion-content">
              <ul>
                <li>Deployable in adverse conditions, such as wastewater and poor weather.</li>
                <li>Carbon-free and eco-friendly. Runs on rechargeable batteries.</li>
              </ul>
            </div>
          </div>
        </div>
        <div class="accordion-tab">
          <div class="accordion-item">
            <input type="radio" id="rad2" name="radio" hidden>
            <label class="accordion-label" for="rad2">Scalable Operations</label>
            <div class="accordion-content">
              <ul>
                <li>Fully autonomous water quality sampling using a network of smart robots.</li>
                <li>Simultaneous coverage over large areas using networked operations powered by SWAN's Bevy Intelligence.</li>
              </ul>
            </div>
          </div>
        </div>
        <div class="accordion-tab">
          <div class="accordion-item">
            <input type="radio" id="rad3" name="radio" hidden>
            <label class="accordion-label" for="rad3">Cost Efficient</label>
            <div class="accordion-content">
              <ul>
                <li>Up to 10x cost savings per sample.</li>
                <li>Minimal need for human intervention.</li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    <!-- </div> -->
    <div class='accordion-container'>
      <img src='{{site.baseurl}}/images/swan-sustainable.png'>
    </div>
  </div>
</div>
<!-- Features -->
<div>
  <div class='four-spacing'></div>
  <div class='row features-row section-margin'>
    <div class='large-6 columns'>
      <div class='swan-intro'>
        <p>Amount of dissolved oxygen in water has immense impact on the aquatic life and hence it is mandated to maintain certain levels of it.</p>
        <div class='spacing'></div>
        <p><span class='title orange'>SWAN</span> can generate alerts based on user settings, when the dissolved oxygen levels go down, and corrective measures can be taken.</p>
      </div>
    </div>
    <div class='large-6 columns'>
      <img src='{{site.baseurl}}/images/swan-aquatic.jpg'>
    </div>
  </div>
  <div class='four-spacing'></div>
  <div class='row features-row section-margin row-padding-bottom'>
    <div class='large-6 columns'>
      <img src='{{site.baseurl}}/images/swan-bgalgae.jpg'>
    </div>
    <div class='large-6 columns'>
      <div class='swan-intro'>
        <p>Algae is a growing concern worldwide and the exposure to blue-green algae and their toxins can cause severe health problems.</p>
        <div class='spacing'></div>
        <p><span class='title orange'>SWAN</span> can determine the blue-green algae levels in the water, which the analysts can visualize and monitor in the SwanViz.</p>
      </div>
    </div>
  </div>
</div>
<!-- Common problems -->
<div>
  <div class='row'>
    <h2 class='section-heading'>Components of <span class='orange'>SWAN</span></h2>
  </div>
  {% for item in site.data.tabs[page.tabs] %}
      {% if item.name ==  "SwanBot" %}
          {% assign checked = "checked" %}
      {% else %}
          {% assign checked = "" %}
      {% endif %}

  <input id="{{ item.input_id }}" name='tab-control' type='radio' class='radio' {{checked}}>
  {% endfor %}
  <div class='type-container'>
      {% for item in site.data.tabs[page.tabs] %}
          <label class='type-item' id="{{ item.id }}" for="{{ item.input_id }}">{{ item.name }}</label>
      {% endfor %}
  </div>
  <div class="tab-panels">
    <div class='row features-row'>
      {% assign tabs = site.pages | where:"categories","swan-component" | sort: "order" %}
      {% for page in tabs %}
      <div id='{{page.tab-id}}' class='tab-panel'>
          {{ page.content }}
      </div>
      {% endfor %}
    </div>
  </div>
</div>
{%- include radio-select.html -%}

<div class='bg-grey'>
  <div class='row'>
    <h2 class='section-heading'>Applications of <span class='orange'>SWAN</span></h2>
  </div>
  <div class='row features-row row-padding-bottom'>
    <div class='large-3 columns swan-features'>
      <div class='media'>
        <i class='icon fab fa-watchman-monitoring'></i>
        <h3>Water quality monitoring</h3>
      </div>
      <p>Visualize realtime water quality data collected from the <span class='orange'>SwanNodes</span>.</p>
    </div>
    <div class='large-3 columns swan-features'>
      <div class='media'>
        <i class='icon fa fa-search-location'></i>
        <h3>Hotspot detection</h3>
      </div>
      <p>Better user experience delivered by wireless data transmission and amazing cloud services.</p>
    </div>
    <div class='large-3 columns swan-features'>
      <div class='media'>
        <i class='icon fa fa-binoculars'></i>
        <h3>Remote surveillance</h3>
      </div>
      <p>Effective spatial and temporal water sampling provided by the <span class='orange'>SwanBots</span> as they are equipped with navigation and sensing.</p>      
    </div>
    <div class='large-3 columns swan-features'>
      <div class='media'>
        <i class='fa fa-fish'></i>
        <h3>Aquaculture</h3>
      </div>
      <p>Effective spatial and temporal water sampling provided by the <span class='orange'>SwanBots</span> as they are equipped with navigation and sensing.</p>      
    </div>
    <div class='four-spacing'></div>
  </div>
</div>
<div>
  <div class='row'>
    <h2 class='section-heading'>Safer environments with <span class='orange'>SWAN</span></h2>
  </div>
  <div class='four-spacing'></div>
  <div class='row features-row section-margin'>
    <div class='large-6 columns'>
      <div class='swan-intro'>
        <p>Amount of dissolved oxygen in water has immense impact on the aquatic life and hence it is mandated to maintain certain levels of it.</p>
        <div class='spacing'></div>
        <p><span class='title orange'>SWAN</span> can generate alerts based on user settings, when the dissolved oxygen levels go down, and corrective measures can be taken.</p>
      </div>
    </div>
    <div class='large-6 columns'>
      <img src='{{site.baseurl}}/images/swan-aquatic.jpg'>
    </div>
  </div>
  <div class='four-spacing'></div>
  <div class='row features-row section-margin row-padding-bottom'>
    <div class='large-6 columns'>
      <img src='{{site.baseurl}}/images/swan-bgalgae.jpg'>
    </div>
    <div class='large-6 columns'>
      <div class='swan-intro'>
        <p>Algae is a growing concern worldwide and the exposure to blue-green algae and their toxins can cause severe health problems.</p>
        <div class='spacing'></div>
        <p><span class='title orange'>SWAN</span> can determine the blue-green algae levels in the water, which the analysts can visualize and monitor in the SwanViz.</p>
      </div>
    </div>
  </div>
</div>
<div>
  <div class='row'>
    <h2 class='section-heading'><span class='orange'>SWAN</span> in the news</h2>
  </div>
  <div class='row features-row section-margin'>
    <!-- <div class='large-12 columns' style='display:flex; flex-wrap:wrap'> -->
      {% assign count = 0 %}
      {% for post in site.posts limit:3 %}
      {% assign isnews = false %}
      {% assign isimage = false %}
      {% if post.external_url != null %}
        {% assign isnews = true %}
      {% endif %}
      {% if post.thumbnail != null %}
        {% assign isimage = true %}
      {% endif %}
      <div class='large-4 columns' id='pulsepage'>
        <div class='mod modBlogPost'>
          <div class='images'>
            {% for image in post.images %}
              <div class='image'><img alt="" src="{{site.url}}/{{image}}" /></div>
            {% endfor %}
          </div>
          <div class='content'>
            <div class='image'>
              <a {% if isnews %}target="_blank"{% endif %} href="{% if isnews %}{{post.external_url}}{% else %}{{site.baseurl}}{{post.url}}{% endif %}">
              <img alt="" src="{% if isimage %}{{site.url}}/{{post.thumbnail}}{% else %}{{site.url}}/{{ site.default_image }}{% endif %}" />
              </a>
            </div>
            <p class='info'>
              <span>{{post.date | date: "%B %d, %Y" }}</span>
            </p>
            <h3 style="text-transform: none;"><a {% if isnews %}target="_blank"{% endif %} href="{% if isnews %}{{post.external_url}}{% else %}{{site.baseurl}}{{post.url}}{% endif %}">{{post.title}}</a></h3>
          </div>
        </div>
      </div>
      {% endfor %}
    <!-- </div> -->
  </div>
  <div class='row row-padding-bottom'>
    <div class='type-container'>
      <a href='{{site.baseurl}}/pulse'><button>View related articles</button></a>
      <a href='{{site.baseurl}}/pulse'><button>Watch our videos</button></a>
    </div>
  </div>
</div>
<div class='bg-grey'>
  <div class='row'>
    <h2 class='section-heading'><span class='orange'>SWAN</span> packages </h2>
  </div>
  <div class='row row-padding-bottom'>
    <div style='display: flex;justify-content: center'>
    <table class='custom-table'>
      <thead>
        <tr>
            <th>Features</th> 
            <th>Standard</th>
            <th>Custom</th>
            <th>Data only</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>24/7 SwanBot usage</td>
            <td><i class='fa fa-check'></i></td>
            <td><i class='fa fa-check'></i></td>
            <td><i class='fa fa-check'></i></td>
        </tr>
        <tr class="active-row">
            <td>Data visualization on UI</td>
            <td><i class='fa fa-check'></i></td>
            <td><i class='fa fa-check'></i></td>
            <td><i class='fa fa-times'></i></td>
        </tr>
        <tr class="active-row">
            <td>Server subscription</td>
            <td><i class='fa fa-check'></i></td>
            <td><i class='fa fa-times'></i></td>
            <td><i class='fa fa-times'></i></td>
        </tr>
    </tbody>
    </table>
  </div>
  </div>
</div>