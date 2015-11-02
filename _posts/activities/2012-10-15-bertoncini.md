---
layout: post
title: "Mario Bertoncini"
excerpt: "80th Birthday Celebration @EMUFest2012"
modified: 2015-11-02T16:39:59
tags: [Bertoncini, Cage, toy, piano, cartridge]
categories: activity
photogalsid: bertonciniphotogal
comments: true
image: 
  feature: 
  credit: 
  creditlink:
 
---

### 2012 October, 9

>Noi musicisti siamo sempre stati schiavi del tempo    
M.B.

***EMUFest***    
*Conservatorio S. Cecilia*, Roma    
EVENTO SPECIALE    
***Per gli ottanta anni di Mario Bertoncini***

 - *Epitaffio in memoria d’un Concerto*, Mario Bertoncini (1968) - 20'
 - *Suite for toy piano*, John Cage (1948) - 8'
 - *Cartridge music*, John Cage (1960) - 18'
 
Performers:  
Piano & Toy Piano *Mario Bertoncini*    
Objects *Federico Scalas*, *Giuseppe Silvi*, *Leonardo Zaccone*

{% for photogals in site.data.photogals %}
![{{ page.title }}]({{ photogals.imagefolder }}DSC_8199.png)
<figcaption>
  SX2DX: Federico Scalas, Giuseppe Silvi, Leonardo Zaccone, Mario Bertoncini, Pasquale Citera, Francesco Bianco, Tommaso Cancellieri.
</figcaption>
{% endfor %}

>Grazie di tutto: delle bellissime espressioni che non so
proprio come io possa aver meritato in così breve tempo; della rapidità con
la quale voi tutti avete saputo reagire non a ciò che io possa aver detto di
"immortale"; senza dubbio alla mia commossa ricezione nei confronti del
vostro entusiasmo per le ragioni della musica! Andate avanti. Lo dico anche
a me stesso, pur non avendo ormai troppo tempo a disposizione (dico questo
non dimenticando gli scongiuri di rito...).
>
Grazie ancora. Un abbraccio corale a voi tutti!
>
MARIO

---

### Photo Gallery

<ul class="th-grid">
{% for photogals in site.data.photogals %}
{% if photogals.id == page.photogalsid %}
{% for image in photogals.images %}

<li><a href="{{ photogals.imagefolder }}{{ image.name }}"><img src="{{ photogals.imagefolder }}_tnb_{{ image.name }}" alt=""></a></li>

{% endfor %}
{% endif %}
{% endfor %}
</ul>
