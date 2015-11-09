---
layout: post
title: "How I did it"
excerpt: "Short report about creating photo-galleries on Jekyll & GitHub Pages"
modified: 
tags: [photo, galleries, how]
categories: blog
comments: true
image:
  feature: 
  credit: 
  creditlink: 
---

<section id="table-of-contents" class="toc">
  <header>
    <h3>Overview</h3>
  </header>
<div id="drawer" markdown="1">
*  Auto generated table of contents
{:toc}
</div>
</section><!-- /#table-of-contents -->

Before starting pushing photos on my website repository I decide to separate
*photogalleries* photos from posts single image content. I created an external
repository to manage photo galleries in separate folders.

## stolen CSS

Before of all, steal something to [Michael Rose](http://mademistakes.com).

{% highlight css %}
#photogallery ul {
  margin: 0;
  padding: 0;
  list-style-type: none;
  text-align: center;
}

#photogallery ul li {
  display: inline;
}

.th-grid {
  display: flex;
  padding-left: 0; // reset
  flex-wrap: wrap;
  li {
    list-style: none;
    flex: auto;
    margin: 0.5vw;
    width: 128px;
  }
  a {
    border-bottom-width: 0 !important; // override
    img {
      // Image hover animation
      transition: transform 0.3s;
      &:hover {
        transform: scale(1.1);
        box-shadow: 0 0 10px rgba($black, .20);
      }
    }
  }
}
{% endhighlight %}

## think in structured data

{% highlight yaml %}
{% raw %}
- id: agalleryid
  imagefolder: https://raw.githubusercontent.com/user-name/repo-name/master/images-parent-folder/the-gallery-folder/
  images:
    - name: imagename.ext
{% endraw %}
{% endhighlight %}

## some lines of LIQUID-HTML

With few lines of ***for*** and ***if*** you can read your *stuctured data* and generate
**HTML** lines. 

{% highlight html %}
{% raw %}
{% if page.photogalsid %}
<h3>Photo Gallery</h3>

<ul class="th-grid">
{% for photogals in site.data.photogals %}
{% if photogals.id == page.photogalsid %}
{% for image in photogals.images %}

<li><a href="{{ photogals.imagefolder }}{{ image.name }}"><img src="{{ photogals.imagefolder }}_tnb_{{ image.name }}" alt=""></a></li>

{% endfor %}
{% endif %}
{% endfor %}
</ul>
<hr />
{% endif %}
{% endraw %}
{% endhighlight %}

## a line of FRONTMATTER

At the FRONTMATTER of your page you need to point the gallery you want include.

{% highlight yaml %}
{% raw %}
---
layout: post
title: "Post Title"
excerpt: "Post Description"
modified: 2015-11-02T16:39:59
tags: [some, tags]
categories: activity
photogalsid: agalleryid
comments: true
image: 
  feature: 
  credit: 
  creditlink:
 
---
{% endraw %}
{% endhighlight %}

