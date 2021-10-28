---
layout: page
title:  M25M series
categories: product-type
tab-id: panel-three
order: 2
---

<h1 class='panel-heading'>M25M SERIES ACOUSTIC MODEMS</h1>
<!-- <h2 class='panel-sub-heading'>High bandwidth applications</h2> -->
<div class='grey-container'>
    <h2 class='edition'>Platinum Edition</h2>
    <ul class="edition-container">
        <li class="modem-container">
            {% assign product_pages = site.pages | where:"categories","modem" %}
            {% for page in product_pages %}
            {% if page.title contains "WNC-M25MPS3" %}
            <div class='mod modBlogPost bg-grey'>
                <a href="{{site.baseurl}}{{page.url}}"><img alt="" src="{{site.baseurl}}/{{page.thumbnail}}"/>
                <div class='content'>
                <h2>Standalone Configuration <br>WNC-M25MPS3</h2>
              </div></a>
            </div>
            {% endif %}
            {% endfor %}
        </li>
        <li class="modem-container">
            {% assign product_pages = site.pages | where:"categories","modem" %}
            {% for page in product_pages %}
            {% if page.title contains "WNC-M25MPE3" %}
            <div class='mod modBlogPost bg-grey'>
                <a href="{{site.baseurl}}{{page.url}}"><img alt="" src="{{site.baseurl}}/{{page.thumbnail}}"/>
                <div class='content'>
                <h2>Embedded Configuration <br>WNC-M25MPE3</h2>
              </div></a>
            </div>
            {% endif %}
            {% endfor %}
        </li>
    </ul>
</div>
<div class='grey-container'>
    <h2 class='edition'>Silver Edition</h2>
    <ul class="edition-container">
        <li class="modem-container">
            {% assign product_pages = site.pages | where:"categories","modem" %}
            {% for page in product_pages %}
            {% if page.title contains "WNC-M25MSS3" %}
            <div class='mod modBlogPost bg-grey'>
                <a href="{{site.baseurl}}{{page.url}}"><img alt="" src="{{site.baseurl}}/{{page.thumbnail}}"/>
                <div class='content'>
                <h2>Standalone Configuration <br>WNC-M25MSS3</h2>
              </div></a>
            </div>
            {% endif %}
            {% endfor %}
        </li>
        <li class="modem-container">
            {% assign product_pages = site.pages | where:"categories","modem" %}
            {% for page in product_pages %}
            {% if page.title contains "WNC-M25MSE3" %}
            <div class='mod modBlogPost bg-grey'>
                <a href="{{site.baseurl}}{{page.url}}"><img alt="" src="{{site.baseurl}}/{{page.thumbnail}}"/>
                <div class='content'>
                <h2>Embedded Configuration <br>WNC-M25MSE3</h2>
              </div></a>
            </div>
            {% endif %}
            {% endfor %}
        </li>
        <li class="modem-container">
            {% assign product_pages = site.pages | where:"categories","wnc" %}
            {% for page in product_pages %}
            {% if page.title contains "WNC-M25MSS3+xCh" %}
            <div class='mod modBlogPost bg-grey'>
                <a href="{{site.baseurl}}{{page.url}}">
                    <h2 class="new-tag"> NEW </h2>
                    <img alt="" src="{{site.baseurl}}/{{page.thumbnail}}"/>
                    <div class='content'>
                        <h2>Multi-Channel Configuration <br>WNC-M25MSS3+xCh</h2>
                    </div>
                </a>
            </div>
            {% endif %}
            {% endfor %}
        </li>
    </ul>
</div>
<div class='grey-container' id='Research'>
    <h2 class='edition'>Research Edition</h2>
    <ul class="edition-container">
        <li class="modem-container"></li>
        <li class="modem-container">
            {% assign product_pages = site.pages | where:"categories","modem" %}
            {% for page in product_pages %}
            {% if page.title contains "WNC-M25MRS3" %}
            <div class='mod modBlogPost bg-grey'>
                <a href="{{site.baseurl}}{{page.url}}"><img alt="" src="{{site.baseurl}}/{{page.thumbnail}}"/>
                <div class='content'>
                <h2>Standalone Configuration <br>WNC-M25MRS3</h2>
              </div></a>
            </div>
            {% endif %}
            {% endfor %}
        </li>
        <li class="modem-container"></li>
    </ul>
</div>