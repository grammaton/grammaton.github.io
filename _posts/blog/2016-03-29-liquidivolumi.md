---
layout: default
title: "Liquidi Volumi ep.ONE"
excerpt: "a way to simulate large electroacoustic concert space"
modified: 2016-03-30T05:34:11
tags: [liquidivolumi, large spece, electroacoustic, concert]
categories: blog
link:
share: true
comments: true
image:
  feature:
  credit:
  creditlink:
---

This is the first attempt to find a way to simulate loudspeakers (in their relative position, distance, environments and WTF.else) for electroacoustic concerts.

![source](https://raw.githubusercontent.com/grammaton/liquidivolumi/master/YCC-LiquidiVolumi-v02/_DeletedItems/media/SourceA.png)

The concert that stimulate this approach will be done next april 22 on 500 meters of *Tiber* river in Rome with acousmatic music (not mine). In this context will be available up to eight channel of music throught eight cluster of Loudspeakers.

My vision to simulate half a kilometer of electroacoustic space concern sure loudspeakers (cluster of it) but in their space context. Obiuvsly.

I've started a project in *Max 6* whit the idea to simulate a starting point with these sound objects:

- sources (eight clusters of loudspeakers)
- clusters:
  - apertures
  - directions
  - back reflections
  - distances
- air, humidity, river banks and water contributions

The longest time I spent on how this simulation could be used, or in what it could be useful.

{% highlight text %}
---/ - - - - - - - 500 meters - - - - - - - - - - - - \---
| |-LEFT BANK------------------------------------------| |
| | . . . walking audience . . .  .   .    ...         | |
|B|                            Mix                     |B|
|R|-----------------------------+----------------------|R|-\
|I| ~   ~   ~   ~   ~   ~   ~   ~   ~   ~   ~   ~   ~  |I| |
|D|   ~   ~   ~   ~   ~   TIBER   ~   ~   ~   ~   ~    |D| 80 meters
|G| ~   ~   ~   ~   ~   ~   ~   ~   ~   ~   ~   ~   ~  |G| |
|E|-+------+------+------+------+------+------+------+-|E|-/
| | H      G      F      E      D      C      B      A | |
| |-RIGHT BANK-----------------------------------------| |
{% endhighlight %}

The goals of this simulation could be:

- predictive speculation of site-specific sound environment
- a way to understand and simulate every kind of environment
- uhm

For this first attempt to explain what this project do, can do, can't do I don't wan't write more.

[This is the jump](https://github.com/grammaton/liquidivolumi.git) to the repo.

The actual development state is an [alpha pre-release v002](https://github.com/grammaton/liquidivolumi/releases).
