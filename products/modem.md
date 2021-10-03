---
layout: default
title: Subnero M25M series modems
banner : images/banner-modem.jpg
thumbnail: images/pulse-thumbnail-ieee-earthzine_grey.jpg
categories: underwatermodem
section_id: products
excerpt: Subnero's software-defined underwater acoustic modems for underwater wireless communication and networking. Subnero's multi-channel modems for data acquisition.
---

<div class='full tall sticky' style='background-image: url({{site.baseurl}}/{{page.banner}});'>
  <div class='row'>
    <div class='large-12 columns'>
    </div>
  </div>
  <div class='spacing'></div>
  <div class='spacing'></div>
  <div class='spacing'></div>
</div>

<div>
    {% for item in site.data.product-tabs %}
        {% if item.name ==  "All Products" %}
            {% assign checked = "checked" %}
        {% else %}
            {% assign checked = "" %}
        {% endif %}

    <input id="{{ item.input_id }}" name='tab-control' type='radio' class='radio' {{checked}}>
    {% endfor %}
    <div class='type-container sticky'>
        {% for item in site.data.product-tabs %}
            <label class='type-item' id="{{ item.id }}" for="{{ item.input_id }}">{{ item.name }}</label>
        {% endfor %}
    </div>
    <div class="tab-panels">
        {% assign product_tabs = site.pages | where:"categories","product-type" | sort: "order" %}
        <div id='panel-one' class='tab-panel'>
            {% for page in product_tabs %}
                {{ page.content }}
            {% endfor %}
        </div>
        {% for page in product_tabs %}
        <div id='{{page.tab-id}}' class='tab-panel'>
            {{ page.content }}
        </div>
        {% endfor %}
    </div>
</div>
{%- include radio-select.html -%}