# Prerequisites

Although the system is ready for you to begin issuing contact and contactless smart cards (the above collectively referred to as just cards) and associated Questions and Answers (Q&A), you should first take some time to plan the manner in which your users and administrators will interface with the system.

A key area to consider is the type of workflows you plan to support. In general, supported workflows include numerous self-service and centralized administration workflows:

* **Self-Service Workflows:** enable your users to complete all but the most secure workflows on their own, without involving the assistance of an administrator or the help desk.  Self-service workflows are considered very secure when coupled with the use of Q&A and/or Authorization Codes. Organizations wanting to decentralize administration and reduce the overall administrative burden on administrators and help desk personnel should consider these workflows.
* **Centralized Workflows:** enable your administrators to maintain fine-grain control over the manner in which your users interface with the system. These workflows are considered more secure, because the user will be required to interface with an administrator or help desk personnel.
* **Hybrid Workflows:** enable your organization to perform common self-service workflows, while centralizing key security workflows, such as offline unblocking of a smart card or resetting Q&A that was forgotten by the user.


In addition to deciding on the type of workflows to support, you must also consider the manner in which your users will interface with the system.  Several key decisions include:

* **Questions & Answers (Q&A):** Q&A can provide an extra layer of security for your environment.  Q&A can be used as either a primary (via Emergency Access with 2FA One Client) or fall-back authentication method to 2FA One Server User Portal. When required within the 2FA One Server User Portal, Q&A enables the ability to utilize secure workflows. This process ensures not only that the user has initially authenticated with a smart card or password to the operating system, but requires the user to submit correct answers to previously established user-selected or administrator-defined questions prior to gaining access to the User Portal. Q&A can be enabled or disabled globally within the Settings menu. When Q&A is used ONLY for Emergency Access it will not be required in the User Portal, unless secure workflows are enabled.
* **Authorization (Auth) Codes:** Auth Codes add an extra level of security to either self-service or centralized workflows. Auth codes can be either given directly to the user by the administrator, security, help desk personnel, or they can be emailed to the user. After receiving the Auth Code, the user must input the Auth Code in the User’s Portal before initiating any task. As with Q&A, Auth Codes can be enabled or disabled globally via the Settings Menu.
* **Integrated Authentication:** Microsoft® Integrated Authentication provides the simplest secure access to both the User and Administrator’s Portals. It is considered the preferred means of authenticating to both; however, it does not provide the added layer of security that Auth Codes do for secure access. By default, 2FA One Server supports Microsoft® Integrated Authentication to both the User and Administrator’s Portals.


Carefully consider which form of authentication is most appropriate for your organization. 

All three authentication methods can be turned on or off at a later date; however, users will develop their overall perceptions of the environment early in the deployment.

This guide provides detailed information on how to configure each of the items discussed above.
