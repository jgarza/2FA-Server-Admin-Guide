# Enroll on Behalf

2FA ONE Server provides the capability for administrators to enroll contact smart cards with PKI and contactless cards on behalf of other users. 

This feature is useful for organizations that want to provide a centralized deployment of 2FA ONE or for specific users, such as executives, who normally do not perform such tasks.

Requirements: 
To perform this task the administrator must be assigned the role of ONE_sys_admin or Security Officer, or the function of Enroll on Behalf must be manually assigned to the Role for which the administrator is logged into 2FA ONE. 

By default, Admin and Helpdesk roles are not permitted to enroll on behalf of other users. 

Additionally, Enroll on Behalf is only available to users with an Authentication Set of Smart Card Only or Contactless Only. 

Enroll on Behalf is NOT enabled for users with Q&A, Emergency Access or Active Directory as a secondary method. 

Finally, the system that you perform an Enroll on Behalf from must be set up the same way as a system on which users perform self-service enrollment. 

###To enroll on the behalf of another user perform the following steps:

1.	Create a new user or move an existing user into the New or Replace Credential States. In the Edit User pop-up, ensure the user is assigned an Authentication Set that includes Smart Card or Contactless only.
3.	Click Save.
3.	The Edit User pop-up will close and the Enroll on Behalf button on the User Information page will be enabled. If the button is not present or is not enabled, please refer back to the requirements above.
4.	Click the Enroll on Behalf button.
5.	Follow the steps in the enrollment wizard.

#### Note: 
Contact smart cards and contactless cards are essentially enrolled the same as when users perform self-service enrollments. The only exception is that you are not required to provide the user’s Active Directory user name and password during Enroll on Behalf for contactless. The user will be required to enter their password the first time they logon with a contactless card.
