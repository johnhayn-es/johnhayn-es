---
layout: post
title: Building Moar Guitars
description: How to tune a website
published: true
category: blog
---

### TL;DR
This is probably the most challenging website build of my career thus far. 

On this project, I had the pleasure of:
* Furthering my understanding of Liquid syntax
* Set up Zapier and Airtable as a CMS via an API
* Writing scripts in Ruby and running them daily using cron jobs

I also made a new friend along the way.


## The Challenge
Earlier this year I set out learning how to build websites on Jekyll. I started by building websites for myself (this portfolio/blog and for the music groups I’m in, [Stacey & John](https://staceyandjohn.co.uk/) and [The Great Fire](https://thegreatfire.co.uk/)). The long term goal is to create my own Jekyll template with documentation that others can use. 

However, before I do that, I wanted to get my head around the intricacies of Liquid and also skill-up in other areas: 
* Javascript for client-side page behaviour
*  Ruby for behind-the-scenes scripts
* Command line tools (better understanding Git deployment, running cron jobs etc)

After the success of building and maintaining a website for my friends at Printers’ Playhouse, I made the decision to find another “client” to build a website for. This would push me to build something to someone else’s specifications and solve problems and challenges with real implications (rather than poking at code for my own ends). 


## The Build
### August 2019: Finding the right client
I first came across [Moar Guitars on Instagram](https://instagram.com/moarguitars) in August 2019 and almost immediately messaged Dan offering to build him a website (Looking back, I’m not sure how I would have delivered it then). It wasn’t until I got back in touch in February 2020 and explained the nature of the project (no need for any compensation) that we finally agreed to go ahead. 

<img src="{{'assets/images/first-contact.PNG' | relative_url }}">

###  March 2020: Work begins
Work began in March and the first month was a good test of working together. Like other recent builds, we started by using the [Forty theme by Andrew Banchich](https://andrewbanchich.github.io/forty-jekyll-theme/) to lay the groundwork:
* We created a shared Google doc where we discussed laid out the content for the site
* I created a custom `Gutiars` page layout, which we’d feed using yaml files - enabling us to use page variables to pull in details and images of each model

By the end of the first four weeks we had a launch-able site, pending a few minor copy amends.


### April 2020: When it fell flat
After about 5 weeks, Dan messaged me to say he had shown the site to his partner for the first time and that he had been thinking about making some fairly fundamental changes to the site.In my eyes, the success of this project relied on having a happy “client” - so, rather than see it as wasted time, I took this as an opportunity to take a step back and look at the site through fresh eyes. 

After discussing what we could do, I spent the next few weeks rolling out some changes to the site:
* Added the ability to switch between hollow and solid-body models on each applicable guitar page, 
* Added an `Optional Extras` element for guitars and bass as an `include` that enabled me to quickly add it to each guitar or bass page


### 1 week from launch 
With less than a week to go, we focused on pulling in content from Dan’s social channels (Instagram and YouTube). At first I eyed-up a Jekyll plugin that, with the right credentials, would enable us to pull through the Instagram content. However, after much frustration as to why it wasn’t working I realised that Github Pages does not allow custom plugins to run. Back to the drawing board. 

Dan was quite keen to help, where he could - so I decided to set up an Airtable account so we could manage the content that we wanted to put into the image gallery. I had a sneaking suspicion that I might be able to use the Airtable API to automatically populate the pages but, while I was familiar with the concept, I had never implemented code to retrieve information from an API before.

After a day fiddling away I managed to:
* Create a Zapier zap that pulls in new Instagram and YouTube content into separate tables in an Airtable Base
* Write Ruby scripts that request from the Airtable API and update the JSON files in the _data folder
* Create separate pages and FOR loops that display content from those files

We then leveraged this approach for the Gallery, Videos and Waitlist pages (the latter being a brilliant idea by Dan to show whose guitars he is currently building).


### May 2020: The Launch & Results
As previously stated, my goal for this pro-bono project was to build a custom site for a “client” that they were happy with. I didn’t expect it to be quite as well-received as it was. 

Dan [launched the site with this video](https://www.instagram.com/p/B_pd42gJ0Yc/) and had two orders come through in the first 48 hours. 

This is what Dan had to say about working together: 

> I have been working closely with John Haynes over the past 3 months to build a website for my business, Moar Guitars.

> He has been so good to work with. 

> I have dabbled in web design myself, and worked with web designers in the past, and what has really set John apart from my past experiences is his keenness to try, and learn, new things. Whenever I came up with an idea that he didn't have an immediate solution for rather then trying to brush the idea to the side, or compromise it ,he seemed to really genuinely enjoy the challenge of figuring out how to make it work. 

>I live in Copenhagen, and John is in Sussex, so we have never met, but working with him remotely has worked very smoothly. Communication is almost instant, always very clear, and positive. 

> A month into the site, and after many many hours of work I decided that the site wasn't targeting my audience, so suggested a redesign. John didn't complain at all. The whole experience has been that he has been trying to make me as happy, and the site as good, as possible, rather then "just getting it done".

> He obviously loves the work, is very good at it and is a genuine pleasure to work with.


