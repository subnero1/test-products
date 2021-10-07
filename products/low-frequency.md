---
layout: page
title:  L5L series
categories: product-type
tab-id: panel-two
order: 1
---

<h1 class='panel-heading'>ACOUSTIC MODEMS - L5L SERIES</h1>
<h2 class='panel-sub-heading'>Low frequency. Long range.</h2>
<div class='grey-container'>
    <h2 class='edition'>Silver Edition</h2>
    <ul class="edition-container">
        <li class="modem-container">
            {% assign product_pages = site.pages | where:"categories","modem" %}
            {% for page in product_pages %}
            {% if page.title contains "WNC-L5LSS3" %}
            <div class='mod modBlogPost bg-grey'>
                <h2 class="new-tag"> NEW </h2>
                <a href="{{site.baseurl}}{{page.url}}"><img alt="" src="{{site.baseurl}}/{{page.thumbnail}}"/>
                <div class='content'>
                <h2>Standalone Configuration <br>WNC-L5LSS3</h2>
              </div></a>
            </div>
            {% endif %}
            {% endfor %}
        </li>
        <li class="modem-container">
            {% assign product_pages = site.pages | where:"categories","modem" %}
            {% for page in product_pages %}
            {% if page.title contains "WNC-L5LSE3" %}
            <div class='mod modBlogPost bg-grey'>
                <h2 class="new-tag"> NEW </h2>
                <a href="{{site.baseurl}}{{page.url}}"><img alt="" src="{{site.baseurl}}/{{page.thumbnail}}"/>
                <div class='content'>
                <h2>Embedded Configuration <br>WNC-L5LSE3</h2>
              </div></a>
            </div>
            {% endif %}
            {% endfor %}
        </li>
    </ul>
</div>