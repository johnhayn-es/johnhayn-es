---
title: Timesheets for high-end television
date: 2023-11-01
category: portfolio
layout: post
---

<div id="1" class="content-section">

## TL;DR
I implemented a new discovery project to help a delivery-focused team deliver a novel timesheets product, tailored specifically to UK film and television production. Now 75% of timesheets (about 1500 per week) are completed and submitted in less than 5 minutes and our product-satisfaction scores are at an all-time high.

![TL;DR Image](https://johnhaynesportfolio.s3.eu-west-2.amazonaws.com/app--check-in--modal--welcome.png){: .scroll-image}
</div>

<div id="2" class="content-section">

## Background
Our strategy was to build a global production finance suite, enabling large studios (like Disney, Netflix, Apple) to hire, manage and pay everyone working across their productions - anywhere in the world. The product vision was simple; roll out our market-leading production management platform gloablly, then connect it to (interchangable) local payroll service(s) to enable us quickly roll out to new international markets. 

Outside of the US & Canada, the UK is the largest territory for Film and Television production spend. Our US counterparts already have timesheets software - but the UK and US workflows are very different and it was decided that we would invest in building a novel service, rather than tailoring the US offering for a UK audience.

### Challenges: 
Three key challenges stood in our way: 
* **Users weren't getting on with our existing timesheets** product; crew (completing timesheets) found it particularly hard to use 
* Production teams were constantly needing to **override incorrect calculations** and, with a new PACT/BECTU (film and tv unions) agreement on the table - we needed to completely revise the underlying calculations engine
* **A number of large contracts were up for renewal** and we needed to work quickly in order to retain current business

Another challenge was the shape of the team. I re-joined the company just as this project was due to kick off and my team consisted of myself (Lead Product Designer), two product managers (each with their own squad of developers) and two product owners (one to work with each of the PMs). As per the org chart, the team was incredibly delivery-focused. While they were all excellent generalists, conducting research was not a core skill for anyone on the team. 

It was clear that we'd need to address this skills gap in order to move at the required pace. 
 
### Objectives
After much consideration we settled on the following objectives for this project: 
* Maximise the Product-satisfaction scores for all key user personas, do this by: 
	* Minimising the time it takes to complete a timesheet
	* Minimise the time it takes to approve timesheets
* Increase the accuracy of timesheets, do this by: 
	* Maximising the accuracy of all hours-to-gross calculations performed by our system
	* Minimise the number of manual overrides required
* Maximise product differentiation from our competitors (give people a reason to switch to us)

![TL;DR Image](https://johnhaynesportfolio.s3.eu-west-2.amazonaws.com/app--check-in--modal--welcome.png){: .scroll-image}
</div>

<div id="3" class="content-section">

## Discovery
When I first joined the team, very little user research had been undertaken. 

Instead, the PMs had focused on categorising inbound feedback into problem statements. While this gave us a solid foundation to start with, I felt uneasy building a completely novel solution solely through the lens of feedback on our existing product. 

I created a [new discovery process]() based on the jobs-to-be-done framework (to identify and prioritise the user needs) and a "definition of done" (to enable us to quantify what differentiated the MVP with the go-to-market version). 

[Image: Discovery process]

After aligning the SVP of Product, I worked to train the PMs on how to implement the process so that we could work in parallel. 

Over the next 3 months: 
* We identified which of the personas were involved
* We deconstructed the end-to-end process (contracts > timesheets > payroll) into more than **50 jobs-to-be-done**
* We conducated **more than 30 hours of primary user research, creating and ranking more than 130 user stories**

[Image: User interviews on-site in Bristol]

### The results
The results were conclusive
Enabled us to break the work into multiple phases
Created a spreadsheet to toggle features in and out of scope
Broke work into milestones

[Image: Spreadsheet for scope]

### Kicking off the project
Brought the whole team together 
Walked through objectives, our findings and the tactical plan
</div>

<div id="4" class="content-section">

## Design iterations and validation
From this point, the project really shifted into delivery mode and I needed to take 25 individual concepts from idea to solution. 

To throw a spanner in the works, there were rumors circulating of an upcoming actors strike. So, coinciding with the end of the discovery process, the UK business decided to pivot to also delivering the first version of our [digital Payroll service](). Work was due to start on this in just 4 weeks time. 

As the sole designer working across both teams, this gave me an incredibly short turnaround time to get initial designs validated and into development. Working closely with the PMs (and working four 80hr weeks in a row) we managed to make incredibly strong progress - 60% of the outstanding work had fully validated refernce designs and everything else was in-progress or descoped into a later milestone. This was achieved by creating open channels with a number of users and regularly re-prioritising what was next based on their feedback. We essentially created an asynchronous focus group of 8-10 Production Accountants and Production Managers who were giving us near real time feedback on the user experience.

Here's a short recap of the most impactful features from this period: 

### Summary chips

#### User story(s)
* As a member of crew, when I am completing my timesheet, I want to know exactly what I am claiming for so that I know I will get paid the correct amount.
* As a member of the production management or finance team, when I am approving a timesheet, I want the totals to be broken down so that I can check for anything that I don't expect

#### Solution
I designed a new component, "chips", to categorise and summarise the durations and financial totals on a timesheet; these components were then embedded into the individual day and weekly summary views:

* Embedded in a sticky panel that scrolls with the user, enabling them to view the detail of the timesheet and determine what contributes to the totals
* Laid out to ensure that the financial total for each section is always visible and enhanced with progressive disclosure to show the detail
* Used accessible labels to highlight when something had been edited by an approver - when clicked, this opens a modal to show which days have been edited

#### Result


### Prepopulation of timesheets 
#### User story(s)
* As a member of crew, when I need to tell the Production Team how many hours I've worked I want to get it done quickly and accurately so that I can get back to my actual job.

#### Solution

#### Result
By implementing this feature: 
* we reduced the minimum number of steps required to complete a timesheet from 33 to just 2
* 75% of our timesheets are completed in 5 minutes or less (about 1500 every week)
* 72% 

### Edited fields
#### User story(s)
* As a member of the production management or finance team, when something has been changed on a timesheet, I want to know what was changed (and by whom) so that I can assess whether or not I need to challenge or amend it.

#### Solution

#### Result

![TL;DR Image](https://johnhaynesportfolio.s3.eu-west-2.amazonaws.com/app--check-in--modal--welcome.png){: .scroll-image}

</div>

<div id="5" class="content-section">

## Summary and reflections
Overall, this project

### Wins
* All of the KPIs were met within 12 months
	* PSAT score of 4.4 out of 5 
	* 75% of timesheets completed in less than 5 minutes
	* 72% of crew agree that Production Portal minimises the time it take to complete their timesheets
	* Average time to approve a timesheet is less than 24 hours
* Implemented a novel product discovery process that has now been adopted across the company (now have nearly 900 user stories documented)
* Up-skilled the product team and gave them fundamental skills that they 

### Challenges
* Should have found a way to avoid the 80 hour weeks

<div class="sticky-container">
  ![Image Description](https://johnhaynesportfolio.s3.eu-west-2.amazonaws.com/app--notifications--messages+grey.png){: .scroll-image}
  ![Image Description](/assets/images/timesheets/chips.jpg){: .scroll-image}
  ![Image Description](/assets/images/timesheets/chips.jpg){: .scroll-image}
</div>

</div>


