# Administering 2FA ONE: Secured Applications

Secured Applications provides a means for organizations to enforce strong and two-factor authentication to applications. Card policies drive the nature in which users authenticate to secured applications. 

Organizations can configure 2FA ONE Client to permit access to secured applications based solely upon the fact that the user authenticated to Windows® with their card, card or Emergency Access, or may elect to defer or strengthen Secured Applications’ authentication events by requiring the user to present their card or card and PIN when authenticating to secured applications. 

To prevent **“the keys to the kingdom”** security shortcoming created by many enterprise Single Sign-on (eSSO) applications, Secured Applications only releases credentials when the user is logged on with their card or Emergency Access (depending on policy). 

An exception to this rule is when the user logged on with user name and password, but is required to present their card or card & PIN when authenticating to secured applications. 

To achieve this functionality, 2FA ONE Client monitors and logs logon events to the system log and drives Card Policy based upon the user’s logon type. 

2FA ONE Client also logs authentication events brokered by Secured Applications. Secured Applications includes the ability for organizations to extend 2FA ONE’s strong and two-factor authentication capabilities to applications that currently have no embedded authentication, such as user name and password authentication. 

As such, with Secured Applications, organizations can now secure the majority of their applications with card or card and PIN security even though the application has no embedded authentication mechanism. 

Secured Applications is optimized for use with Citrix®applications, such as Citrix®Receiver, Citrix®Program Neighborhood Agent, and Citrix®browser-based products. Secured Applications is further designed to enhance the securability and usability of VMware®View by direct integration, allowing seamless launching, authentication and roaming of virtual machines. 

This section will provide you with an overview on how to look up and manage Secured Applications. 
Before you can provision a Secured Applications template from 2FA ONE Server, you must first configure the template in 2FA ONE Client and synchronize with 2FA ONE Server. 
See the 2FA ONE Client Administrator Guide for information on how to create Secured Applications templates
