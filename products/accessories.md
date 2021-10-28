---
layout: default
title: Subnero Modem Accessories
banner : images/banner-accessories.jpg
thumbnail: images/thumbnail-accessories.png
categories: product-type
section_id: products
excerpt: Optional upgrades and accessories for Subnero underwater modems.
tab-id: panel-four
order: 3
---

<h1 class='panel-heading'>Optional Accessories and Upgrades</h1>
<!-- <h2 class='panel-sub-heading'>Enhanced performance</h2> -->
<div class='grey-container'>
	<h2 class='edition'>Battery Packs</h2>
	<ul class="edition-container">
		<li class="modem-container">
			{% assign product_pages = site.pages | where:"categories","accessories" %}
			{% for page in product_pages %}
				{% if page.title contains "Primary Battery Packs" %}
	        	<div class='mod modBlogPost bg-grey'>
		        	<a href="{{site.baseurl}}{{page.url}}"><img alt="" src="{{site.baseurl}}/{{page.thumbnail}}"/>
		          	<div class='content'>
		            <h2>Battery Packs</h2>
		          </div></a>
		        </div>
	        	{% endif %}
	        {% endfor %}
		</li>
	</ul>
</div>

<div class='grey-container'>
	<h2 class='edition'>Electrical Upgrades</h2>
	<ul class="edition-container">
		<li class="modem-container">
			{% assign product_pages = site.pages | where:"categories","accessories" %}
			{% for page in product_pages %}
				{% if page.title contains "Coprocessor" %}
		        <div class='mod modBlogPost bg-grey'>
		        	<a href="{{site.baseurl}}{{page.url}}"><img alt="" src="{{site.baseurl}}/{{page.thumbnail}}"/>
		          	<div class='content'>
		            <h2>Co-processors</h2>
		          </div></a>
		        </div>
	        	{% endif %}
	        {% endfor %}
		</li>
		<li class="modem-container">
			{% assign product_pages = site.pages | where:"categories","accessories" %}
			{% for page in product_pages %}
				{% if page.title contains "Sensors" %}
		        <div class='mod modBlogPost bg-grey'>
		        	<a href="{{site.baseurl}}{{page.url}}"><img alt="" src="{{site.baseurl}}/{{page.thumbnail}}"/>
		          	<div class='content'>
		            <h2>Sensors</h2>
		          </div></a>
		        </div>
	        	{% endif %}
	        {% endfor %}
		</li>
		<li class="modem-container">
			{% assign product_pages = site.pages | where:"categories","accessories" %}
			{% for page in product_pages %}
				{% if page.title contains "Storage" %}
		        <div class='mod modBlogPost bg-grey'>
		        	<a href="{{site.baseurl}}{{page.url}}#embedded"><img alt="" src="{{site.baseurl}}/{{page.thumbnail}}"/>
		          	<div class='content'>
		            <h2>Storage</h2>
		          </div></a>
		        </div>
	        	{% endif %}
	        {% endfor %}
		</li>
		<li class="modem-container">
			{% assign product_pages = site.pages | where:"categories","accessories" %}
			{% for page in product_pages %}
				{% if page.title contains "Interfaces" %}
		        <div class='mod modBlogPost bg-grey'>
		        	<a href="{{site.baseurl}}{{page.url}}#embedded"><img alt="" src="{{site.baseurl}}/{{page.thumbnail}}"/>
		          	<div class='content'>
		            <h2>External Interfaces</h2>
		          </div></a>
		        </div>
	        	{% endif %}
	        {% endfor %}
		</li>
	</ul>
</div>

<div class='grey-container'>	
	<h2 class='edition'>Mechanical Upgrades</h2>
	<ul class="edition-container">
		<li class="modem-container">
			{% assign product_pages = site.pages | where:"categories","accessories" %}
			{% for page in product_pages %}
				{% if page.title contains "Hulls" %}
		        <div class='mod modBlogPost bg-grey'>
		        	<a href="{{site.baseurl}}{{page.url}}"><img alt="" src="{{site.baseurl}}/{{page.thumbnail}}"/>
		          	<div class='content'>
		            <h2>Hull Options</h2>
		          </div></a>
		        </div>
	        	{% endif %}
	        {% endfor %}
		</li>
		<li class="modem-container">
			{% assign product_pages = site.pages | where:"categories","accessories" %}
			{% for page in product_pages %}
				{% if page.title contains "Cables" %}
		        <div class='mod modBlogPost bg-grey'>
		        	<a href="{{site.baseurl}}{{page.url}}"><img alt="" src="{{site.baseurl}}/{{page.thumbnail}}"/>
		          	<div class='content'>
		            <h2>Cables</h2>
		          </div></a>
		        </div>
	        	{% endif %}
	        {% endfor %}
		</li>
		<li class="modem-container">
			{% assign product_pages = site.pages | where:"categories","accessories" %}
			{% for page in product_pages %}
				{% if page.title contains "Mechanical Accessories" %}
		        <div class='mod modBlogPost bg-grey'>
		        	<a href="{{site.baseurl}}{{page.url}}#embedded"><img alt="" src="{{site.baseurl}}/{{page.thumbnail}}"/>
		          	<div class='content'>
		            <h2>Mechanical Accessories</h2>
		          </div></a>
		        </div>
		       {% endif %}
	        {% endfor %}
		</li>
	</ul>
</div>
