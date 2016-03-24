# Allow Synchronization of Non-Domain Users

Allow synchronization of non-domain users is enabled by default. This setting enables administrators to limit the ability of non-domain users to synchronize their data to 2FA ONE Server. This setting applies to local users and users located in other domains. 

**Note: **	Synchronization is limited by the domain user name and password pair. In the event a local account contains the same user name and password pair as one located in the domain (local = user1/password and domain - user1/password) the users data will synchronize to 2FA ONE Server. Two accounts will be created on 2FA ONE Server, one with the local account information and one with the domain account information. Administrators can distinguish between the two accounts based upon the domain representation in the user lookup menu



