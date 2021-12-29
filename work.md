---
title: Work
category: work
layout: post
---

# Fyld
**Strategic Design Lead**

I'm joining the Fyld team in February 2022.

----

# We Got POP
**Senior Product Designer**

I joined POP to help build a smarter, fairer entertainment industry. 

I lead the design team and am the principal designer on the Production Portal, a service that production companies use to manage their productions. Features include contracting, messaging, timesheets and reports.

Due to the nature of the projects I'm working on, I'm unable to publish a lot of my most recent work.

### Notable projects

* Payroll Service
* Production Portal
* Distro

----


# YourWelcome
**Head of Growth, then Head of Product**

As Head of Growth I helped launch [YourWelcome ↗] [2]{:target="_blank"} worldwide, from launch to 30 territories in less than seven months. I was asked to lead the product team, introducing a set of ecommerce and messaging features that remain the foundation of the business today.

### Notable projects

* YourwWelcome Advance
* Verifying guest emails


## YourWelcome Advance

**Project outline and my role**

In the Vacation Rental industry it’s incredibly valuable to verify your guests prior to check-in as it helps to protect against fraudulent bookings. 

Each Online Travel Agency offers differing levels of protection, but ultimately it is the accommodation provider’s responsibility to protect themselves.

YourWelcome Advance was built to enable hosts to ask guests for their contact details and government-issued ID in advance, as well as taking a means of payment to cover any damaage or in-property purchases.

As the product lead I oversaw the specification and roll-out of this new product line. On this occasion I was also the principle designer, working with a key client to bring the idea to fruition, from MVP to general release. As the CPO I researched and prepared the pricing and go-to-market strategy.

**Current check-in process**

1. Guest books the accommodation, usually via an Online Travel Agent
2. Pre-arrival communication; this usually consists of a mixture of manual and automated messaging. While most OTAs remove or obscure phone numbers and email addresses from the on-platform message, many accommodation providers had found ways around this in order to communicate directly. e.g. replacing the ‘@’ with (at) when spelling their email
3. Guest travels to the property; guests often get lost on their way, or underestimate the time required to travel - missing their original ETA and, in some cases, costing the host additional hours while their meet and greet team is left waiting for them to arrive
4. Confirmation that the guest has arrived; in the vast majority of cases, this required the guest to confirm they had arrived via message - which sometimes wouldn’t come until the next day


### Field study

I organised and attended research sessions with the front-office staff from two of our largest clients, who described their ideal check-in solution.

> “It should be simple for the guests and for us”

> “Depending on the type of guest, it should ask them for different information”

> “It should offer our upgrade services in advance”

> “We could send them all the information they need to get in to the property, like the door codes”

### The MVP

After quickly mocking up a number of screens and using card sorting sessions to determine an appropriate order, we put together a live MVP to trial this new feature. 

The first version of the online check-in form included the following screens: 

1. Capture and verify up-to-date contact details
2. Capture their government-issued ID details and photo (at which point the form is submitted)
3. Up-sell services prior to arrival (optional)
4. Provide detailed instructions to find and enter the property (optional)

![Yourwelcome Advance MVP](../assets/images/yourwelcome-advance--mvp.png)

**Results**

YourWelcome Advance became one of the company's most sought-after products. 

Based on a short trial in 200+ properties it was estimated that, on average, properties with YourWelcome Advance would protect against 1 fraudulent booking every 2 months and provide an increase in up-sell value of $10-15 per booking.

YourWelcome has since pivoted to offer a software-only version of their service (via Propertycare.com) and YourWelcome Advance remains part of the key offering.


___

## Verifying guest emails

We were planning to release an online check-in/account portal for guests to manage their booking(s), view/purchase services and manage their data. Email verification was a necessary precursor to the release of this new platform, to ensure that we could securely communicate sensitive information to guests.

Another challenge faced by accommodation providers are the proxy email addresses used by Online Travel Agents for their internal messaging systems. The proxy system use addresses such as `john34566@guest.airbnb.com`; the internal systems obsure links, email addresses and URLs – making it hard to communicate with the guest.

![Guest Check-In](https://johnhaynesportfolio.s3.eu-west-2.amazonaws.com/app--check-in--modal--welcome.png)

**Objective(s)**

* Verify guest emails upon their arrival at the property
* Encourage guests to edit proxy emails
* Build a process that can be easily recycled in the upcoming online check-in/guest dashboard product
* Do so, without negatively affecting the completion rate of the check-in screens

**Design**

The app uses the primary guest’s email to validate that they are who they say they are, with a view to pre-filling details from their booking – expediting the check-in process. Anyone that fails to validate their email is treated as a new guest, and made to complete the entire check-in form.

The secure check-in flow is simple:
1. The guest guest arrives and proceeds to check-in using email verification
2. An email is sent, containing a verification link
3. The guest verifies their email address by tapping the button in the body of the email
4. The tablet is unlocked and the guest can proceed to check-in

The secure check-in was released as an opt-in feature to existing users; we made the decision to do this after reviewing feedback from a previous change to the check-in screens where users were not notified. Secure check-in is the default option for all new users. When the tablet detects a proxy email address, the guest is prompted to update their email. The guest submits & verifies an email they can access during their stay – and if they agree to further communication, meaning accommodation providers can re-market to their guests.

Watch the secure check-in process in action:

<iframe width="560" height="315" src="https://www.youtube.com/embed/fbrxIgafArI" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

**Results**

* One week after launch, the secure check-in had been adopted by around half of YourWelcome’s users (opt-in) – which is higher than the projected number.
* Completion rates of check-in screens initially decreased by ~5%, but after improving the on-screen messaging we actually saw check-in completions rise by 1.2% above their original rate
* One month after launch, around 800 proxy email addresses had been converted to real, verified emails



___

## Instant messaging with guests

This feature was prioritised after inbound requests increased, following a period of significant growth. The resulting Slack app is something that I’m hugely proud of; not only did we exceed the original objectives, but this feature has enabled our customers to provide a significantly better experience for their guests.

![Messages](https://johnhaynesportfolio.s3.eu-west-2.amazonaws.com/app--notifications--messages+grey.png)

**Objective(s)**

* Make it easy for anyone to connect their Slack & YourWelcome accounts
* Allow hosts to message their guests, in real time, sharing photos and links
* Customise the experience to make it clear to hosts & guests who they are speaking to

**Design**

We built a slack app that connects to Slack’s Real Time Messaging API. The app is self-installed by YourWelcome’s customers via the Slack marketplace. The app is simple to use and has useful features designed to help our customers manage this new communication channel:

* All properties that a user wants to connect to Slack appear as individual channels, enabling our customers to manage who from their team is involved in conversations at a per-property level
* We replace the bot user’s name with the name and language of the guest, making it easy to personalise the chat and to anticipate any language barriers
* The tablet app wipes the chat history on device with each new reservation so that guests cannot see previous conversations, but the full conversation is retained in Slack for the property manager

**Results**

Instant messaging is a polarising feature. For some of our customers, the thought of more communication with their guests goes against the reason they bought the tablets in the first place. For others, this feature has become key to their day-to-day operations. Our Slack app has proven to be a key driver of customer retention.

* 22% properties using YourWelcome have messaging enabled
* 50% lower response times for clients
* 94% customers more likely to renew their subscription at the next billing date

**Links**

* [Blog](https://www.yourwelcome.com/%e2%9c%89-you-have-1-new-message/)
* [Supporting docs](https://www.yourwelcome.com/help/connected-accounts/slack/)


## Reservations calendar

It became clear that the YourWelcome tablet would become a much more powerful tool if we were able to attribute in-app behaviour to a particular guest. This would provide a wealth of guest data that we now take for granted.

![calendar](https://johnhaynesportfolio.s3.eu-west-2.amazonaws.com/Calendar+-+booking+slide.png)

**Objective(s)**

Users should be able to create, edit and delete a variety of events in a calendar.

The calendar system is used to:

* View & edit bookings
* View & approve service requests
* Setting custom reminders
* Integrate with external reservations calendars (HomeAway, Booking.com etc)

The calendar will be integrated with other external calendars; guest reservations will be imported from third parties, so the system must adhere to web standards (such as ISO 8601, handling timezones).

**Result**

The calendar has become the backbone of a number of systems in the YourWelcome ecosystem.

* Can integrate 7+ external calendars, including HomeAway and Booking.com
* Enables property managers to sell of late check-outs, via YourWelcome services

**Impact**

This key feature has enabled us to link in-app events to individual bookings; we now customise the guest’s experience based on past behaviour, as well as providing more detailed sales and analytical reporting to our clients.

* ~10000+ reservations added/imported per month in 2018
* 70% YourWelcome customers have connected a third party calendar
* Late check-outs have become YourWelcome’s most-sold additional service


**Links**

* [Supporting docs](https://www.yourwelcome.com/help/calendar/)


___

## Personalised experiences

A majority of short-term rental hosts manage their property remotely, so the touchpoints between them and their guests are few and far-between (and can often feel very formal). 

YourWelcome's self check-in options enable property hosts to provide a warm welcome to guests and capture vital details, in the guests' first language. 

![Property Rating](https://johnhaynesportfolio.s3.eu-west-2.amazonaws.com/app--check-in--modal--rating.png)

**Objective(s)**

* Provide a platform to personally welcome guests
* Collect vital information upon arrival, such as expected departure time
* Provide a platform to sell in-stay services and extensions to the booking
* Translation options for guests from overseas

**Design**

The check-in screens are fully customisable; hosts can choose which screens appear and in what order. Each screen itself is customiable, enabling hosts to capture the information required by their business.

By tying the check-in screens to YourWelcome's Services platform, hosts are able to create exclusive check-in products. If they have a property calendar connected, they're even able to sell additional nights in the property. 

![Guest Preferences](https://johnhaynesportfolio.s3.eu-west-2.amazonaws.com/app--check-in--modal--guest-interests.png) ![Check-Out Time](https://johnhaynesportfolio.s3.eu-west-2.amazonaws.com/app--check-in--modal--checkout-date.png)


___

## GDPR compliant stays

In order to help our clients adhere to GDPR, YourWelcome needed to introduce new features in our app and dashboard. Survey results indicated that clients were confused by what GDPR was, whether it affected them and how to ensure their business was compliant.

**Objective(s)**

Due to the perceived complexity of GDPR, the feature should:

* Be clear and simple for Guests to use
* Be simple to set up by hosts, enabling our clients to become fully compliant with GDPR
* Ensure that YourWelcome adheres to GDPR

**Result**

We created a configurable check-in screen, managed via the dashboard, that enables YourWelcome and our clients to explain to guests how we capture and store their data. The app screen includes a dynamic list of data points (and corresponding checkboxes) that the guest must view and agree to before they can complete their check-in.

Guests must scroll through the list and tap the checkboxes to demonstrate that they agree to the items within – they cannot complete their check-in without completing all mandatory fields.

**Impact**

* At the time this feature was release YourWelcome was seeing an average of 5000 check-ins per month; >85% of check-ins are fully GDPR compliant
* YourWelcome is GDPR compliant

**Links**

* [Blog](https://www.yourwelcome.com/gdpr)
* [Supporting docs](https://www.yourwelcome.com/help/data-collection-gdpr-controls/)


# Pearlshare

**Growth Lead, then UX Lead**

Pearlshare was a B2C iOS app for creating and sharing travel guides. I joined Pearlshare to lead user acquisition & retention for Pearlshare's  iOS app. I led the redevelopment of the onboarding experience, instant messaging and launched pearlshare.com.


___

## Location Picker

The goal of this design was to allow a user to add or update an address of a Pearl in as few steps as possible. Storing the location of a Pearl requires users to add both an address, and potentially a different geocoded location (while the two values are often the same, they are treated as independent values). Apple sometimes misinterprets the address and places the map pin in the wrong place - so we needed to introduce a flow that would involve as few steps as possible to add a new address and location, while still allowing the user to update each value independently. 

![Location Picker](https://johnhaynesportfolio.s3.eu-west-2.amazonaws.com/IMG_4761.PNG)

The solution was to use alerts that offer the user the option of overriding the value of the address or location, after one or other has been updated. This reduces the number of steps required to add both an address and location from scratch - while maintaining the option to update each value separately.


___

## Pearlshare.com

The goal of this design was to allow a user to add or update an address of a Pearl in as few steps as possible. Storing the location of a Pearl requires users to add both an address, and potentially a different geocoded location (while the two values are often the same, they are treated as independent values). Apple sometimes misinterprets the address and places the map pin in the wrong place - so we needed to introduce a flow that would involve as few steps as possible to add a new address and location, while still allowing the user to update each value independently. 

The solution was to use alerts that offer the user the option of overriding the value of the address or location, after one or other has been updated. This reduces the number of steps required to add both an address and location from scratch - while maintaining the option to update each value separately.


# On Tap

**Digital Project Manager**

I joined On Tap to oversee their more complex Magento eCommerce projects through to delivery, managing an off-shore team of 4. Clients included Bettys & Taylors, Party Pieces (Middleton Family) and Academia


# James Grant Group 

**Junior Multimedia Producer, then Multimedia Producer, then Project Manager: Hairy Bikers' Diet Club**

I produced and developed online content for broadcast talent including Ant & Dec, Fearne Cotton, Holly Willougby, Philip Schofield, the Hairy Bikers and many more

* [Hairy Bikers' Diet Club](../work/hairy-bikers)