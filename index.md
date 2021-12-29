---
layout: home
title: About me
category: about
image: '../assets/images/john.png'
--- 

{% assign reversed_posts = site.posts %}{% for post in reversed_posts | limit:1 %}{% if post.categories contains "blog" %}I sometimes write about work. Most recently, I have written about <a href="{{ post.url }}">{{post.title | downcase}}</a>.{% endif %}{% endfor %}


I've held a number of key product and design roles over the last 8 years. I'm interested in the future of work & travel and previously held an advisory positions at Govia Thameslink (2015 and 2019) and London Water-Enabled Transport (2016-2017). You can see all other the jobs I’ve had on my [LinkedIn profile ↗] [5]{:target="_blank"}.



[1]: https://wegotpop.com 
[2]: https://www.wegotpop.com/pages/uk/production/
[5]: https://www.linkedin.com/in/johnmahaynes/
[6]: https://www.printersplayhouse.co.uk
[7]: https://www.moarguitars.com
[8]: https://www.thegreatfire.co.uk