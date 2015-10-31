---
layout: post
title: "Mario Bertoncini"
excerpt: "Career Celebration during EMUFest 2012"
modified: 2015-10-31T01:31:17
tags: [Bertoncini, Cage, toy, piano, cartridge]
categories: activity
photogalsid: bertonciniphotogal
comments: true
image: 
  feature: 
  credit: 
  creditlink:
 
---

### 2012 October, 15

***EMUFest***    
*Conservatorio S. Cecilia*, Roma

 - *Epitaffio in memoria d’un Concerto*, Mario Bertoncini
 - *Suite for toy piano*, John Cage
 - *Cartridge music*, John Cage
 
 Piano & Toy Piano:    
 *Mario Bertoncini*
 
 performers:    
 *Federico Scalas*    
 *Giuseppe Silvi*    
 *Leonardo Zaccone*
 
 ---

{% for photogals in site.data.photogals %}
  {% if photogals.id == page.photogalsid %}
    {% for image in photogals.images %}
![{{ page.title }}]({{ photogals.imagefolder }}{{ image.name }})
    {% endfor %}
  {% endif %}
{% endfor %}

<!-- <figure class="third">
	<img src="/images/image-filename-1.jpg">
	<img src="/images/image-filename-2.jpg">
	<img src="/images/image-filename-3.jpg">
	<figcaption>Caption describing these three images.</figcaption>
</figure> -->