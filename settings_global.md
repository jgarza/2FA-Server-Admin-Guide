# GLOBAL SETTINGS OVERVIEW
2FA ONE Server is installed with the following default settings:

1.	Authorization Codes are Suppressed.
2.	Secure Workflows are Enabled.
3.	Role Mapping is Not Enabled.
4.	Auto Enroll is Turned Off
5.	Allow synchronization of non-domain users is Enabled.
6.	Allow Self-Service of reset credential during validation is NOT Enabled

**Note:** The logic within 2FA ONE Server is to always attempt to authenticate an Authorization Code when the need arises. Therefore, suppressing authorization codes has the true effect of having 2FA ONE Server always assume the user entered their authorization code already and that it was correct. 

This increases convenience for the end users and administrators, while reducing security. This is especially apparent if secure workflows are enabled and if an authentication set is used which has no secure workflows present (such as Smart Card only). 

A user attempting to reset their credential (such as unblocking a card) will be able to do so without being prompted for any additional information. 

Therefore, if this option is suppressed, take care to assign only authentication sets with Secure Workflows question set can be used for Emergency Access onto users’ systems with 2FA ONE Client. 

You can still change the policy for this access, but not the actual question set.

### Globally Suppress Auth Codes

The use of Authorization or Auth Codes will add an extra level of security to either self-service or centralized workflows. 

Auth codes can either be given directly to the user by the administrator, security, or help desk personnel, or they can be emailed to the user. 

Upon receipt, the user will be required to input the Auth Code in the User’s Portal before initiating any tasks for which another authentication method is not available (e.g. when entering a “New Credential” or “Reset All Credentials” workflow). 

Auth Codes can be enabled or disabled globally.

To change the Auth Code global setting in the system (on or off), perform the following tasks:

1.	Select the Suppress Auth Code link.
2.	Check mark the Always suppress authorization code
3.	Click the Save button to commit changes or the Cancel button to exit.

**Note:**	
Self-service is still possible, even with auth codes enabled. This does require that the system has been properly configured to communicate with an SMTP server. 

When that is the case, if the user requests a self service workflow that would normally require an auth code, the option to e-mail the auth code directly to the user is available. 

This is similar to how many online systems offer password retrieval or other security information transmissions. 

In this way, by virtue of the user having access to his or her email account, it is still possible to provide a more secure self-service, and not require the burden of administration.

### Secure Workflows

The Global Settings submenu provides the capability to configure secure workflows. 

Secure workflows require the user to answer the defined secure workflow method (generally Q&A) before being permitted to perform secure workflows (Unblock Card, Change Q&A, Replace Card) within the User’s Portal; however, the user can perform changes to personal settings.

**Note:**	
In general, the easy way to understand the difference between a “secure” workflow and a “normal” workflow is to understand whether or not the user has to validate that particular credential prior to modifying it. 

For example, Change PIN requires the user to validate their current PIN before changing it to a new one. On the contrary, Unblock PIN (or Reset PIN) assumes the user cannot validate their current PIN (because it is blocked). 

In this scenario, simply setting a new PIN would be considered a “secure” workflow. It is similar to the difference in Active Directory between a user changing their password versus resetting the password. 

To enable this functionality select the check box and click Save. This functionality is a global setting and will apply to all workflows. It can be turned on or off at a later date, as long as a secure workflow method has been previously defined.

When 2FA ONE Server is deployed with multiple credentials being managed, any authentication method can be used in place of Q&A for this purpose, provided that the authentication method is defined for Secure Workflow within the corresponding authentication set for a user.


### Role Mapping

Role Mapping refers to the ability to map 2FA ONE Server Roles to Active Directory groups. This has been explained in detail under section 8.4.


### Auto Enroll

Auto Enroll refers to the ability to allow users which already exist in Active Directory to automatically be enrolled in 2FA ONE Server upon first access to the 2FA ONE Server User Portal. 

###Update Database Settings

Use this link to update settings related to your database, such as: Server Name, Database Name, ID, and Password.



---


#### ***Special Note - DATABASE ADMINISTRATORS***

In addition to the database settings which can be set here from within the 2FA ONE Server Administrator Portal, we also provide the following DATABASE-ONLY keys:

**IgnoreAllDomains: **for use when syncing if you want to treat all users just based on username only.  This can be useful if one username may need to authenticate across many different domains, or if domains are causing issues due to dns renaming constraints or netbios issues.

**AutoCreate:** will automatically create a user that attempts to sync up, based on the AutoEnroll settings in the portal.

**UseEnhancedPinPolicy:** Tells the server to enforce CJIS PIN Policy as found in CJIS authentication policy dated XXXXX (need to look that up, or the version number)

**TestConnectionPassword:** Useful for verifying with some third party hardware (load balancers and such) if the server is alive and responding correctly, based solely on html responses.  This is the password that should be supplied for validation.  Simply call the url: http://servername/one/validation_portal/dovalidate.aspx?test=1 and it should return with a validation page for “TestConnection” if successful.  This page will not allow an actual login.

**EnableSendSMSforOTP:** If this is true, a user can send “sms” or “text” as their password and have an OTP texted to them for use in their next attempt.  I just emailed this in an instruction to Shiva.

**UseBioKeyWebKey:** If this is true, 2FA ONE Server will use settings found in the restservices\web.config in order to integrate with BioKey’s WebKey product.



---


### Update Mail Server Settings

Use this link to update settings related to your mail server, such as: SMTP Server Name, Port, Default “From” Address, User name, Password, and whether or not to Ignore Certificate Errors.

### Allow PingMe for OTP Users
This option enables the mobile (PUSH) Authentication method from within the 2FA ONE Mobile OTP App.

### Require PIN for PingMe
This option, when set, requires that users enter a PIN along with their password when authenticating using PingMe.

### Allow Unauthenticated One-To-Many Biometric Match

### Allow Synchronization of non-domain users
Allow synchronization of non-domain users is enabled by default. This setting enables administrators to limit the ability of non-domain users to synchronize their data to 2FA ONE Server. This setting applies to local users and users located in other domains. 

**Note: **	Synchronization is limited by the domain user name and password pair. In the event a local account contains the same user name and password pair as one located in the domain (local = user1/password and domain - user1/password) the users data will synchronize to 2FA ONE Server. 

Two accounts will be created on 2FA ONE Server, one with the local account information and one with the domain account information. Administrators can distinguish between the two accounts based upon the domain representation in the user look-up menu.

### Allow Self-Service of Reset Credential During Validation
This enables a link on validation pages that allows a user to state they have forgotten that credential (such as “I forgot my PIN”. Clicking it will immediately put the user in reset credential state.

### Send an E-Mail When Sending an SMS

### Administrator's Portal

Type the permanent URL of your 2FA ONE Server Admin portal. This will be used by the system in email alerts and auth code notifications to direct users or administrators to the appropriate URL.

http://[servername]/ONE/admin_portal/default.aspx

### External Provisioning Link for Mobile Clients

Type the server name of your 2FA ONE Server Admin portal. This will be used by the system in provisioning mobile clients (iOS, Android, Windows) for use with our 2FA ONE Mobile App.

http://[servername]/ONEService/Provision.aspx


