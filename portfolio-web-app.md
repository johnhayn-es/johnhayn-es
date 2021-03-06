---
title: Web App
description: Opening the pearly gates
date: 2014-01-01
image: 'https://johnhaynesportfolio.s3.eu-west-2.amazonaws.com/Calendar+-+booking+slide.png'
categories: [portfolio, design]
project: Pearlshare
layout: item
nav-menu: false
show_tile: true
---

The goal of this design was to allow a user to add or update an address of a Pearl in as few steps as possible. Storing the location of a Pearl requires users to add both an address, and potentially a different geocoded location (while the two values are often the same, they are treated as independent values). Apple sometimes misinterprets the address and places the map pin in the wrong place - so we needed to introduce a flow that would involve as few steps as possible to add a new address and location, while still allowing the user to update each value independently. 

### Results
The solution was to use alerts that offer the user the option of overriding the value of the address or location, after one or other has been updated. This reduces the number of steps required to add both an address and location from scratch - while maintaining the option to update each value separately.