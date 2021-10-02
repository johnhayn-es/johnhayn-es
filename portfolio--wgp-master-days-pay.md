---
title: Master Day's Pay
description: A payroll system to coll
date: 2021-05-01
image: '../assets/images/wgp-mdp--master-days-pay.png'
categories: [portfolio, strategy]
project: We Got POP
layout: item
nav-menu: false
show_tile: false
---


## Problem 
Production accounts often need to make adjustments to what someone is due to be paid in their upcoming payroll. However, each crew member's weekly pay can be derided from multiple timesheets and other standalone payments. The adjustment might affect how much overtime and holiday the crew member is owed, so it's important to take all payment sources into account when making the adjustment. 

Production accountants work in teams and often need to be audited, so it's important that everybody can see all the changes that have been made. 

The Master Day's Pay solution aims to provide a clear, visual way to view the delta of all payment sources and provide users with the tools they need to make accurate adjustments to the total pay an individual is due for any given day they've worked.

### My role 
I worked alongside the Product Director as the sole product designer on this project to conduct over 40 hours of user interviews over a three-months, then produce prototype iterations as we start preparing for general release. POP has recently been acquired by Entertainment Partners who have built and maintained the incumbent accountancy products used by the industry. They have just given us (the POP team) the green light to bring our new payroll product to market.

## What the accountants were saying...

>> “It’s hard to consolidate all the information”
>> “I need to be able to make quick amendments to individuals, or in bulk”
>> “Adjustments sometimes require approval”
>> “The whole thing needs to be easy to audit”

## Approach

### Consolidating disparate payment sources, for multiple individuals

The Master Day’s Pay is the master record where everything that affects how much an individual is being paid are consolidated. 
The UI enables accountants to view the gross amounts that everyone associated to a production on any given day. From this screen they can view:

* All payment sources; the deal (which sets the day-rate), any timesheets the crew member has completed, on-set reports (these carry information about overtime)
* Any adjustments or amendments that have been made for payroll

[!A screenshot depicting the user interface design for Master Day's Pay](../assets/images/wgp-mdp--master-days-pay.png)

### Making adjustments

Accountants regularly need to adjust the amount that someone is being paid - they may get a call from a Line Producer to let them know that a whole department has done an hour of overtime, or that a specialist camera operator was needed for an exta day because of inclement weather.

Adjustments are made from the Master Day’s Pay screen.

Selecting a row loads the consolidated gross amounts for an individual. The accountant can make amendments by overriding the value in the field - overridden fields are shown with a yellow background (colour coding from our design system).

To make amendments in bulk, the user can select multiple rows. Where fields are an exact match, the value is shown. When there are multiple values for a field, the word `multiple` is shown in place of the values. If the accountant overrides a field with multiple values, all of them are updated to the new value.

All adjustments are reflected on the Adjustments tab.

[!A screenshot depicting the user interface design for making adjustments](../assets/images/wgp-mdp--adjustments.png)

## Summary

### Solution
Accountants aren’t the only ones that need visibility of the adjustments process - Line Producers and other members of the Production office may need to approve changes before they go to payroll. 

The adjustments summary is a separate tab, available as a standalone page, that enables any approvers to quickly see which fields were changed. The ‘minus’ row show the previous value and the ‘plus’ rows show the new value.

[!A screenshot depicting how users can tell which lines have been modified, added or removed](../assets/images/wgp-mdp--summary.png)

### Results
This iteration of Master Day’s Pay has been accepted into the backlog and is currently in build to become part of our MVP. Once the MDP is released, we will commence the next stage of user testing with the network of users that we have been accruing in the last two months - it’s critical that the accountants in our network are able to test this before using it in a live environment. 