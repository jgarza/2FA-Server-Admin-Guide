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

Role Mapping refers to the ability to map 2FA ONE Server Roles to Active Directory groups. This has been explained in detail under section **XXXXXXXX****


### Auto Enroll

Auto Enroll refers to the ability to allow users which already exist in Active Directory to automatically be enrolled in 2FA ONE Server upon first access to the 2FA ONE Server User Portal. 

Auto Enrollment Options:

* Enable Auto-Enrollment of users with Integrated Windows Authentication
* SELECT Default Authentication Set (Default is Contactless + Emergency Access
* SELECT Default Role (Default is User)
* SELECT Default Language (Default is English)

###Update Database Settings

Use this link to update settings related to your database, such as: Server Name, Database Name, ID, and Password.

### Update Mail Server Settings

Use this link to update settings related to your mail server, such as: SMTP Server Name, Port, Default “From” Address, User name, and Password.






