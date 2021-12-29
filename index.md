---
layout: home
title: About me
image: '../assets/images/john.png'
---

## I work with teams to design game-changing products & services through thoughtful research, value-based design strategy and hands-on collaboration. In the last 8 years I have held a number of key product and growth roles in small, fast-moving businesses. I'm joining [Fyld ↗] [1]{:target="_blank"} in the New Year as Strategic Design Lead. 

{% assign reversed_posts = site.posts %}
{% for post in reversed_posts | limit:1 %}
{% if post.categories contains "blog" %}
I sometimes write about work. Most recently, I have written about <a href="{{ post.url }}">{{post.title | downcase}}</a>.
{% endif %}
{% endfor %}

You can see all other the jobs I’ve had on my [LinkedIn profile ↗] [5]{:target="_blank"}.


I enjoy running and staying fit. I'm interested in the future of work & travel and previously held an advisory positions at Govia Thameslink (2015 and 2019) and London Water-Enabled Transport (2016-2017). I play guitar for [The Great Fire ↗] [8]{:target="_blank"}. I build and maintain websites for my friends: [Printer’s Playhouse ↗] [6]{:target="_blank"} and [Moar Guitars ↗] [7]{:target="_blank"}.



[1]: https://wegotpop.com 
[2]: https://www.wegotpop.com/pages/uk/production/
[5]: https://www.linkedin.com/in/johnmahaynes/
[6]: https://www.printersplayhouse.co.uk
[7]: https://www.moarguitars.com
[8]: https://www.thegreatfire.co.uk