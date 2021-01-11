---
layout: post
title: Visual Guitar Designer
description: A custom guitar design for Instagram
published: true
categories: [Design, Jekyll]
---

After taking delivery of my very own <a href="https://moarguitars.com/guitars/wayfair/">Moar Guitars Wayfair</a>, I felt that the standard order form on the site didn't really do the guitar justice. I got in touch with Dan and we began work on a <a href="https://moarguitars.com/design-wayfair/">visual guitar designer</a>.

We set out our desired functionality: 

* People can visually design their own Wayfair
* Once they've selected the options they want, they can give their guitar a name and save the image to their camera roll
* All of the options for each completed design should be saved somewhere, for us to review later (and analyse for patterns)

While the concept is simple, I'd never if-statements with this many variables before and knew it would push me. I'd like to add a caveat that I am definitely an experienced javascript-er and the solutions I've put together are heavily, heavily bodged. If you know of ways that I can simplify or improve my code, I am very open to hearing how it could be done. 

<image src="../assets/images/full-size-guitar.png"/>

## The Guitar Design
I used photos of the guitars to create an illustration using Adobe XD, which I saved as an SVG. I decided to go with a simple visual style and selected a palette of colours to represent the different wood and metal finishes. 

I created a large HMTL form, broken into tabs, to enable the user to control the design of the guitar. Every update triggers a javascript function that recalculates how each layer behaves. 

Dan's Guitars are made of the same groups components and I've detailed how I handled each of them below.

#### The Neck
The design for this component is usually the same for all of Dan's guitars. This is positioned to align with the right-side of the container. All other components are position relative to the neck's position. The original intention was to add multiple body types (an idea we will revisit in the future).

Users can specify the neck and fretboard wood, which changes the colour of the component. 

#### The Body
Like the neck, the body can be made from a number of select woods - the colour of the main body shape is updated based on what the users selects. I also added a limited number of wood grain details to attempt to reflect the finished result. 

The Wayfair bodies are completely hollow and usually have a pair of matching f-holes - but this is not mandatory. The user uses a checkbox to determine which of the f-holes to include in their design. 

#### Binding
The headstock, neck, body and f-holes can all be individually bound with white or black binding. 

#### Hardware 
Users can select from a number of hardware options. The type of tailpiece chosen will sometimes limit the accompanying bridge - this is controlled by setting and disabling certain fields using an IF statement. 

Users can also define the colour of the hardware; gold or silver. 

#### Electronics & Controls
Once a user had selected the type and quantity of pickups they want to add, they can select the exact positioning on the body using a slider. This updates the position of the pickup, relative to the neck. 

The user can define the layout of the controls and how many potentiometers to includes. 

## Saving Finished Designs
Dan and I started work on this with intention of capturing the finished designs - so that we could share them on Instagram and analyse the component choices made for potential future stock builds. 

I set up some additional fields so users can give their design a name and share their instagram handle and posted the results to Airtable each time this is done.

I had originally attempted to save and post an actual image, but found it almost impossible to do this completely in the client. Instead, I opted for a simpler solution - I concatenated all of chosen options like url parameters in a hidden string and posted that instead. I built Dan a hidden page with a form that enables him to decode the string and visualise the design. He then posts screenshots of this to Instagram instead. Slightly more work - but it works.  

## The Test
Working with Dan is great - he was keen to get a good-enough version out of the door to see what people though. 

After hours of fiddling, I got the design and form to a place where we were ready to go. The decoder wasn't working and it was still a little buggy (the pickups had a funny way of just completely breaking occassionally) - but we shipped it. 

24 hours and one instagram post later, 50 guitars had been created. We were onto something and Dan's audience we're lapping it up. 

Here are a few of my favourite designs including "ArsenWenge", "The Sheridan" and, my favourite, "Murray's Big Boy".

<image src="../assets/images/guitar-designs.png"/>

## Next Steps
Since the initial release, we've tidied things up a bit. I got the decoder working and we've started work to analyse the trends. 

Dan's got a number of ideas about what we can add - but there's a few other things we want to do before we turn our attention back to the visual designer. Until then, it's quietly sitting on the site, generating Instagram content and data that we can look at whenever we like. 
