---
layout: post
title: SEO for Github Pages
---

You've got Github Pages up and running, installed your Jekyll theme and added a custom domain. Your site is looking great, but when you're looking for it on Google (as you hope so many others are) you can't find any trace if it. 

This is exactly what happened to me with [my band's website](https://thegreatfire.co.uk)

In this article I've laid out everything that I've done to help my Github Pages site rank on Google.  

## How do I get my Github Pages site to rank on Google?
This is a very good question and one I was struggling to answer. I'm not new to the concept of SEO; while I've been part of projects that have done work to implement search-engine-friendly strategies, I've never done the hands-on implementation. 

> None of this would be possible without the helpful advice of my friend [Luke Smith](https://www.lukesmithseo.co.uk/). He's an SEO Expert and helped me round-off a lot of the ideas that I've implemented. 


## The Technical Stuff
### Page Header: Meta and Open Graph
Before I got too carried away creating content for the site, I wanted to make sure that the site's structure was optimised to help the content perform as best it could. 

I updated the page header as below.

<code>
	<title>{{ site.title }}</title>
	<meta name="description" content="{{ page.seo_description }}"/>
	<meta charset="utf-8" />
	<meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no" />
	<!--[if lte IE 8]><script src="{{ "assets/js/ie/html5shiv.js" | relative_url }}"></script><![endif]-->
	<link rel="stylesheet" href="{{ "assets/css/main.css" | relative_url }}" />
	<!--[if lte IE 9]><link rel="stylesheet" href="{{ "assets/css/ie9.css" | relative_url }}" /><![endif]-->
	<!--[if lte IE 8]><link rel="stylesheet" href="{{ "assets/css/ie8.css" | relative_url }}" /><![endif]-->
	<!-- Open Graph -->
	<meta property="og:locale" content="en_GB">
	<meta property="og:type" content="article">
	<meta property="og:title" content="{%if page.title %}{{ page.title }}{% else %}{{ site.title }}{% endif %}">
	<meta property="og:url" content="{{ site.url }}{{ page.url }}">
	<meta property="og:image" content="../assets/images/the-great-fire-band--og-image.png" />
	<meta property="og:site_name" content="{{ site.title }}">
	<meta property="article:publisher" content="http://www.facebook.com/greatfireband" />
	<meta property="article:author" content="https://www.facebook.com/greatfireband" />
	<meta property="article:published_time" content="{{ page.date }}" />
	<meta property="og:description" content="{% if page.description %}{{ page.description }}{% else %}{{ site.description }}{% endif %}">
	<!-- Favicon -->
	<link type="image/x-icon" sizes="180x180" href="../images/the-great-fire--sussex-cover-band--favicon-100.ico">
	<link rel="icon" type="image/png" href="../assets/images/the-great-fire--sussex-cover-band--favicon-32.png" sizes="32x32">
	<link rel="icon" type="image/png" href="../assets/images/the-great-fire--sussex-cover-band--favicon-16.png" sizes="16x16">
</code>

Let's take a look at what I did: 

* As my template uses `page.description` elsewhere in the template, I include a new page element, `page.seo_description`, which enabled me to control how the page would appear when indexed
* I've added Open Graph tags; these help boost SEO and control how the page appears in link previews on sites like Facebook, Twitter and LinkedIn
* I created a specific image to appear via Open Graph - I'll later update this to include an `if` statement to use the page image, if one exists
* I made sure the site has a favicon for different resolutions (they're used be different devices); each image title is optimised

### Google Tech and My Business Listing
Google's ecosystem is intrinsically linked, so I made an effort to explicitly link as much of it together as possible:

* I Installed Google Analytics on our site
* I verified the domain in Google's Search Console, then requested indexing
* I verified our site's link to our YouTube channel, where we'll be posting all of our videos
* I registered the band on Google My Business

### Github Repo Settings
Google is also pushing to make SSL standard across the web and is punishing insecure sites. After you've enabled your custom domain on the Github repo, make sure you check the `secure with SSL` check box - this will generate an SSL certificate for your site. 

### Sitemap
The Jekyll theme I chose doesn't come with a sitemap, so I had to generate my own. I did this using the `jekyll-sitemap` plugin ([available via Github](https://github.com/jekyll/jekyll-sitemap)). After it was created, I submitted the sitemap URL to Google Search Console and checked it was working correctly. 


## Optimising the Site Content
### Search Term Research
I am trying to improve the ranking of my band's website, so I made a note of the terms that people might be using to look for bands like ours: 

* Sussex cover _or_ function band
* Live music Eastbourne
* Sussex Wedding Band

The first thing I did was take a quick look at the competition. Thankfully, other bands in the area either had relatively simple sites or no website at all. 

### SEO Tools
People use search engines to find answers to their questions (hell, you may have found this page doing this). One of the simplest SEO strategies to help your page show in results is to create content for your site that answers these questions (this got meta real quick, huh?). 

I used a few tools to help me get a picture of all the related questions and search terms that may apply. 

* [Answerthepublic](hrrps://https://answerthepublic.com/); a great tool for exploring all of the questions that relate to your key terms
* [SEO Moz](https://moz.com/); even their free tools provide a lot of value - you can use this to view the potential traffic of each search term 

### The Basics
With a better understanding of the key words my targeted audience were likely to be using, I started to optimise the site content.

* I started working SEO terms into the text on the site's pages and posts
* I gave all the images on my site relevant file names and ensured they had descriptive alt tags (this has the added bonus of making the site more accessible to those using screen readers, too!)


### External Links & Social Media Accounts 
Back links help bring traffic to your site - the obvious place to start is by updating all of your social accounts to link back to your site as you can.

* I made sure all of our social profiles point back to our site
* I tested the Open Graph tags by creating a post on Facebook and pinning it to the top of our Facebook page


### SEO-targeted page(s)
I've started to create pages that specifically target SEO terms that relate to our band. This content is designed to actually be useful to the audience and answer the most common questions that people are searching for. 

* I used my research to inform the template of the article, including as many related questions as I could - then answering them!
* I also published details of other local bands that don't have websites websites - I'm hoping that, by mentioning them on our site, our review/recommendation of them could index

## Next Steps
There's still a few thing left to do: 

* Youtube videos; obviously we'll post clips of the music we play, but I also want to shoot some videos targeting the questions our audience will ask. YouTube videos are rich in meta info and should make a significant difference to those pages (I think the videos themselves rank within the results, so should help with domain authority on the topic)
* Optimising the Open Graph content to include `if` statements, to pull in the page/post content when it's there
* More pages! One for each of the most popular groups of terms

I hope that there's something on this page that you found useful - feel free to [hit me up on Twitter](https://twitter.com/johnhayn_es) if there's anything you want to discuss. 