# RECYCLE CARD UTILITY

The Recycle Card Utility provides an administrator the ability to identify ownership of a contact smart card, or an enrolled contactless card. 

Once the cardholder is identified, the credential can be returned to the owner, or the card can be cancelled within 2FA One Server, or if the cardholder is not in the Steady State, the Recycle Card Utility can format and reset the card to factory defaults so that it may be re-issued to a new cardholder.

The Recycle Card Utility is installed with 2FA One Server and an OMNIKEY reader must be connected to the 2FA One Server. To recycle a card you must run the utility locally from: <drive>:\Program Files\2FA\One Server\tools\RecycleCard.exe

To Recycle a card do the following:

* Navigate to the install folder (<drive>:\Program Files\2FA\ONE Server\Tools\RecycleCard)
* Right click on RecycleCard application and select Run as administrator.
* Insert a contactless or contact smart card.
* Click the Connect button.
* The utility will display Card Name, Serial Number and Assigned user. 
* If the card is associated with a user in Steady State you will be prompted to edit the user’s state in 2FA ONE before recycling the card.
* If the card is not associated with a 2FA One user, you will be prompted to confirm intent to format the card.
* If you have not attempted to issue this card from 2FA One, then it is recommended that you click No and allow 2FA One to manage the card from this point.
* If you have failed to issue the card from within 2FA One, or you have other reason to format this card, then click Yes.
