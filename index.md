---
layout: home
title: About me
image: '../assets/images/john.png'
---

# John Haynes

I work with teams to design game-changing products & services through thoughtful research, value-based design strategy and hands-on collaboration.

This site hosts my portfolio and blog, where I document things I create and share my thoughts about design.

{% assign reversed_posts = site.posts %}
{% for post in reversed_posts | limit:1 %}
{% if post.categories contains "blog" %}
Most recently, I have written about <a href="{{ post.url }}">{{post.title | downcase}}</a>.
{% endif %}
{% endfor %}

I enjoy running and staying fit. I'm interested in the future of work & travel and previously held an advisory positions at Govia Thameslink (2015 and 2019) and London Water-Enabled Transport (2016-2017). I play guitar for [The Great Fire ↗] [8]{:target="_blank"}. I build and maintain websites for my friends: [Printer’s Playhouse ↗] [6]{:target="_blank"} and [Moar Guitars ↗] [7]{:target="_blank"}.

## Career

In the last 8 years I have held a number of key product and growth roles in small, fast-moving businesses. I'm currently  Senior Product Designer at [We Got POP ↗] [1]{:target="_blank"}, where I lead the design team and am the principal designer working on the [Production Portal ↗] [2]{:target="_blank"}. 

I am highly motivated and thrive in a fast-paced environment with an air of uncertainty. I am an adept and versatile supporting player, the sort of person that start-up founders seek as a key early employee.

My career to date combines three interconnected disciplines; design, strategy and storytelling. 

This combination enables me to do the work I do today:

* Principles; establishing the fundamental purpose of the design function within the organisation
* Strategy; simple, value-based strategies to help the organisation reach its goals
* Research; surfacing insights quickly so that the team can make faster decisions
* Product & service design; building effective and efficient solutions
* Measuring value; analysing the impact of the changes we make

You can see all the jobs I’ve had on my [LinkedIn profile ↗] [5]{:target="_blank"}.


[1]: https://wegotpop.com 
[2]: https://www.wegotpop.com/pages/uk/production/
[5]: https://www.linkedin.com/in/johnmahaynes/
[6]: https://www.printersplayhouse.co.uk
[7]: https://www.moarguitars.com
[8]: https://www.thegreatfire.co.uk