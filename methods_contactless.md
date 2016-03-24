# Contactless Card Method

The Contactless Card sub-menu enables you to configure profiles and policies for contactless cards. 

Within the Contactless Card submenu there are four submenus, they are:

1.	**Profile List:** Provides an overview of the configured Contactless Profiles, including the configured PIN
policy, card behavior options, and PIN required/not-required settings.
2.	**PIN Policies:** Provides the ability for organizations to establish PIN usage policies and selection criteria for securing contactless cards protected with a PIN.
3.	**New Profile:** Provides the ability for organizations to create custom profiles that can pair PIN policy with
Sets and assigned to users.
4.	**New PIN Policy:** Provides the ability to create custom PIN policies for contactless card authentication.

### Profile List

By default, 2FA ONE Server has a single profile for contactless cards. 

The Default profile contains the following settings:

1. Default PIN Policy of:
  3.	Attempts before PIN becomes blocked = 3
  4.	Minimum PIN Length = 4
  5.	No more than three repeated characters
  6.	No more than three consecutive characters
2.	Card Behavior set to:
  3.	TAP IN/OUT
  4.	Lock Workstation
3.	PIN Use Policy set to – Require PIN
4.	Secure Logon Password - No

### PIN Policy

The PIN policy sub-menu provides the ability for organizations to create custom PIN policies and edit out-of-the-box PIN policies. 

By default there are four PIN policies with varying degrees of security from High to Low. 

The default PIN Policy contains a policy based upon best practices. PIN Policy can be edited or you can create your own PIN policy. 

PIN policy is assigned to a Profile that can be assigned to a Set; then, the Set can be assigned to a user. 


### New Profile

In order to assign a new Profile to a Set you must first create the new Profile. 

To create a new Profile, click the New Profile link and the New Contactless Card Profile pop-up will appear. In the example the new Profile name is “Contactless Sample” and the following settings were configured:

1.	PIN Policy – Default
2.	Card Behavior – Tap In / Tap Out, Lock Workstation
3.	Require PIN for Workstation Logon
4.	Do NOT Require PIN for Workstation Unlock

### New PIN Policy

In order to assign a new PIN Policy to a Profile you must first create the new PIN Policy. To create a new PIN Policy, click the New PIN Policy link, and the Create New PIN Policy pop-up will appear. 

You must name the new policy and select your desired settings.

1.	Attempts until the PIN is blocked = numeric value
2.	Number of PINs to Keep in History = numeric value
3.	Minimum PIN Length = numeric value
4.	Maximum PIN Length = numeric value
5.	PIN Expiration Days = numeric value
6.	PIN Complexity Requirements
  7.	No more than three repeated characters
  8.	No more than three consecutive characters
  9.	Must contain alpha and numeric characters
  10.	Must only contain numeric characters
  11.	Must contain special characters
