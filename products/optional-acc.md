---
layout: page
title:  Optional Accessories
categories: accessories
tab-id: panel-four
---

<h1 class='panel-heading'>Optional Accessories and Upgrades</h1>
<div class='grey-container'>
    <ul class="edition-container">
        <li class="modem-container"></li>
        <li class="modem-container">
            {% assign product_pages = site.pages | where:"categories","accessories" %}
            {% for page in product_pages %}
            {% if page.title contains "Subnero Modem Accessories" %}
            <div class='mod modBlogPost bg-grey'>
                <a href="{{site.baseurl}}{{page.url}}">
                    <h2 class="new-tag"> NEW </h2>
                    <img alt="" src="{{site.baseurl}}/{{page.thumbnail}}" />
                    <div class='content'>
                        <h2>Accessories</h2>
                    </div>
                </a>
            </div>
            {% endif %}
            {% endfor %}
        </li>
        <li class="modem-container"></li>
    </ul>
</div>