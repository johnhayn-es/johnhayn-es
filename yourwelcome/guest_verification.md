---
layout: post
nav-menu: false
show_tile: false
---

<span class="breadcrumbs">[Portfolio](../portfolio) / [YourWelcome](../yourwelcome) / Guest Verification</span>

# Guest Verification
We were planning to release an online check-in/account portal for guests to manage their booking(s), view/purchase services and manage their data. Email verification was a necessary precursor to the release of this new platform, to ensure that we could securely communicate sensitive information to guests.

Another challenge faced by accommodation providers are the proxy email addresses used by Online Travel Agents for their internal messaging systems. The proxy system use addresses such as `john34566@guest.airbnb.com`; the internal systems obsure links, email addresses and URLs – making it hard to communicate with the guest.

![Guest Check-In](https://johnhaynesportfolio.s3.eu-west-2.amazonaws.com/app--check-in--modal--welcome.png)

### Objective(s)

* Verify guest emails upon their arrival at the property
* Encourage guests to edit proxy emails
* Build a process that can be easily recycled in the upcoming online check-in/guest dashboard product
* Do so, without negatively affecting the completion rate of the check-in screens

### Design
The app uses the primary guest’s email to validate that they are who they say they are, with a view to pre-filling details from their booking – expediting the check-in process. Anyone that fails to validate their email is treated as a new guest, and made to complete the entire check-in form.

The secure check-in flow is simple:
1. The guest guest arrives and proceeds to check-in using email verification
2. An email is sent, containing a verification link
3. The guest verifies their email address by tapping the button in the body of the email
4. The tablet is unlocked and the guest can proceed to check-in

The secure check-in was released as an opt-in feature to existing users; we made the decision to do this after reviewing feedback from a previous change to the check-in screens where users were not notified. Secure check-in is the default option for all new users. When the tablet detects a proxy email address, the guest is prompted to update their email. The guest submits & verifies an email they can access during their stay – and if they agree to further communication, meaning accommodation providers can re-market to their guests.

Watch the secure check-in process in action:

<iframe width="560" height="315" src="https://www.youtube.com/embed/fbrxIgafArI" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Results

* One week after launch, the secure check-in had been adopted by around half of YourWelcome’s users (opt-in) – which is higher than the projected number.
* Completion rates of check-in screens initially decreased by ~5%, but after improving the on-screen messaging we actually saw check-in completions rise by 1.2% above their original rate
* One month after launch, around 800 proxy email addresses had been converted to real, verified emails