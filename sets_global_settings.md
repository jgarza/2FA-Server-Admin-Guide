# Global Settings

This sub-menu allows you to configure the authentication policy for Secured Workflows. 

The Global Settings submenu provides the capability to configure secure workflows. 

Secure workflows require the user to answer the defined secure workflow method (generally Q&A) before being permitted to perform secure workflows (Unblock Card, Change Q&A, Replace Card) within the User’s Portal; however, the user can perform changes to personal settings.

For example, Change PIN requires the user to validate their current PIN before changing it to a new one. On the contrary, Unblock PIN (or Reset PIN) assumes the user cannot validate their current PIN (because it is blocked). 

In this scenario, simply setting a new PIN would be considered a “secure” workflow. It is similar to the difference in Active Directory between a user changing their password versus resetting the password. 

To enable this functionality select the check box and click Save. This functionality is a global setting and will apply to all workflows. It can be turned on or off at a later date, as long as a secure workflow method has been previously defined.

When 2FA ONE Server is deployed with multiple credentials being managed, any authentication method can be used in place of Q&A for this purpose, provided that the authentication method is defined for Secure Workflow within the corresponding authentication set for a user.

**Note:**	
In general, the easy way to understand the difference between a “secure” workflow and a “normal” workflow is to understand whether or not the user has to validate that particular credential prior to modifying it. 




