# Directory Mapping

The Directory Mapping sub-menu provides the capability to map 2FA ONE Server Roles to Active Directory Groups. This feature enables your predefined groups in Active Directory to inherit the associated 2FA ONE Server Roles, thereby eliminating the requirement to manage roles within multiple applications. 

You do not have to map every role to an AD group, you may elect to map only one role to an AD group. 

To map a 2FA ONE Server Role to an Active Directory Group:
1.	Check the Enable Directory Mapping check box. 
2.	Enter the corresponding Directory Group Name (full DN) in the text box to the right of the appropriate 2FA ONE Server Role. When this function is enabled, any user who is a member of the Directory Group will be treated as a member of the 2FA ONE Server Role. Alternatively, you can click the Directory Lookup Tool icon and navigate to the desired Active Directory group. 
  3.	Note: In order to enter multiple groups, thereby assigning all of those groups to a particular Role, you will need to separate each DN by a semicolon “ ; ”. 
3.	Click Save to commit your changes or Cancel to exit the menu. 

### Best Practice:
For administrators desiring to only manage roles from within Active Directory, it is best practice to assign all 2FA ONE Server user accounts the basic “User” Role.

Then, allow Group Membership within Active Directory to determine elevated privileges. 

Keep in mind that permissions are
additive. Therefore, if a user is a member of multiple groups, he or she will receive all of the cumulative permissions of each associated 2FA ONE Server Role. 

Thus, in order to maintain proper role separation, take care not to have users in groups in Active Directory which would violate your desired role separation within 2FA ONE Server.
