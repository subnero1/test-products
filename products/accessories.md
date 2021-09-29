---
layout: page
title: Subnero Modem Accessories
banner : images/banner-accessories.jpg
thumbnail: images/thumbnail-accessories.jpg
categories: product-type
section_id: products
excerpt: Optional upgrades and accessories for Subnero underwater modems.
tab-id: panel-four
order: 3
---

<h1 class='panel-heading'>Optional Accessories and Upgrades</h1>
<div class='grey-container'>
	<h2 class='edition'>Battery Packs</h2>
	<ul class="edition-container">
		<li class="modem-container">
			<div class="hOXnHC">
				{% assign product_pages = site.pages | where:"categories","accessories" %}
					{% for page in product_pages %}
					{% if page.title contains "Primary Battery Packs" %}
		        <div class='mod modBlogPost'>
		        	<a href="{{site.baseurl}}{{page.url}}"><img alt="" src="{{site.baseurl}}/images/thumbnail-batterypack.jpg" />
		          	<div class='content'>
		            <h2>Battery Packs</h2>
		          </div></a>
		        </div>
		        {% endif %}
		        {% endfor %}
			</div>
		</li>
	</ul>
</div>

<div class='grey-container'>
	<h2 class='edition'>Electrical Upgrades</h2>
	<ul class="edition-container">
		<li class="modem-container">
			<div class="hOXnHC">
				{% assign product_pages = site.pages | where:"categories","accessories" %}
					{% for page in product_pages %}
					{% if page.title contains "Coprocessor" %}
		        <div class='mod modBlogPost'>
		        	<a href="{{site.baseurl}}{{page.url}}"><img alt="" src="{{site.baseurl}}/images/thumbnail-coprocessor.jpg" />
		          	<div class='content'>
		            <h2>Co-processors</h2>
		          </div></a>
		        </div>
		        {% endif %}
		        {% endfor %}
			</div>
		</li>
		<li class="modem-container">
			<div class="hOXnHC">
				{% assign product_pages = site.pages | where:"categories","accessories" %}
					{% for page in product_pages %}
					{% if page.title contains "Sensors" %}
		        <div class='mod modBlogPost'>
		        	<a href="{{site.baseurl}}{{page.url}}"><img alt="" src="{{site.baseurl}}/images/thumbnail-sensors.jpg" />
		          	<div class='content'>
		            <h2>Sensors</h2>
		          </div></a>
		        </div>
		        {% endif %}
		        {% endfor %}
			</div>
		</li>
		<li class="modem-container">
			<div class="hOXnHC">
				{% assign product_pages = site.pages | where:"categories","accessories" %}
					{% for page in product_pages %}
					{% if page.title contains "Storage" %}
		        <div class='mod modBlogPost'>
		        	<a href="{{site.baseurl}}{{page.url}}#embedded"><img alt="" src="{{site.baseurl}}/images/thumbnail-storage.jpg" />
		          	<div class='content'>
		            <h2>Storage</h2>
		          </div></a>
		        </div>
		        {% endif %}
		        {% endfor %}
			</div>
		</li>
		<li class="modem-container">
			<div class="hOXnHC">
				{% assign product_pages = site.pages | where:"categories","accessories" %}
					{% for page in product_pages %}
					{% if page.title contains "Interfaces" %}
		        <div class='mod modBlogPost'>
		        	<a href="{{site.baseurl}}{{page.url}}#embedded"><img alt="" src="{{site.baseurl}}/images/thumbnail-rs232.jpg" />
		          	<div class='content'>
		            <h2>External Interfaces</h2>
		          </div></a>
		        </div>
		        {% endif %}
		        {% endfor %}
			</div>
		</li>
	</ul>
</div>

<div class='grey-container'>	
	<h2 class='edition'>Mechanical Upgrades</h2>
	<ul class="edition-container">
		<li class="modem-container">
			<div class="hOXnHC">
				{% assign product_pages = site.pages | where:"categories","accessories" %}
					{% for page in product_pages %}
					{% if page.title contains "Hulls" %}
		        <div class='mod modBlogPost'>
		        	<a href="{{site.baseurl}}{{page.url}}"><img alt="" src="{{site.baseurl}}/images/thumbnail-hull.jpg" />
		          	<div class='content'>
		            <h2>Hull Options</h2>
		          </div></a>
		        </div>
		        {% endif %}
		        {% endfor %}
			</div>
		</li>
		<li class="modem-container">
			<div class="hOXnHC">
				{% assign product_pages = site.pages | where:"categories","accessories" %}
					{% for page in product_pages %}
					{% if page.title contains "Cables" %}
		        <div class='mod modBlogPost'>
		        	<a href="{{site.baseurl}}{{page.url}}"><img alt="" src="{{site.baseurl}}/images/thumbnail-cables.jpg" />
		          	<div class='content'>
		            <h2>Cables</h2>
		          </div></a>
		        </div>
		        {% endif %}
		        {% endfor %}
			</div>
		</li>
		<li class="modem-container">
			<div class="hOXnHC">
				{% assign product_pages = site.pages | where:"categories","accessories" %}
					{% for page in product_pages %}
					{% if page.title contains "Mechanical Accessories" %}
		        <div class='mod modBlogPost'>
		        	<a href="{{site.baseurl}}{{page.url}}#embedded"><img alt="" src="{{site.baseurl}}/images/thumbnail-mechanical.jpg" />
		          	<div class='content'>
		            <h2>Mechanical Accessories</h2>
		          </div></a>
		        </div>
		        {% endif %}
		        {% endfor %}
			</div>
		</li>
	</ul>
</div>
