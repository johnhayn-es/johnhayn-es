---
title: pearlshare.com
date: 2015-04-01
category: portfolio
layout: post
---

The goal of this design was to allow a user to add or update an address of a Pearl in as few steps as possible. Storing the location of a Pearl requires users to add both an address, and potentially a different geocoded location (while the two values are often the same, they are treated as independent values). Apple sometimes misinterprets the address and places the map pin in the wrong place - so we needed to introduce a flow that would involve as few steps as possible to add a new address and location, while still allowing the user to update each value independently. 

The solution was to use alerts that offer the user the option of overriding the value of the address or location, after one or other has been updated. This reduces the number of steps required to add both an address and location from scratch - while maintaining the option to update each value separately.