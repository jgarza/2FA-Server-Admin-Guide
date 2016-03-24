# Key Backup Tool

When 2FA ONE Server is installed, random encryption keys are generated and that will be used to securely communicate with clients and store protected data in the system. Because of how this data is encrypted and decrypted, each database will be tied to its corresponding Server Key. It is always advised to back up your keys after installation and during any server operation that may affect the server keys.

Additionally, for 2FA One Server deployments where multiple application (IIS) Servers are to be deployed to communicate with a single SQL instance or farm, each 2FA One Server must utilize the same encryption keys in order to access encrypted data stored in the database.

2FA provides a Key Backup Tool that is provided to backup the key from your initial 2FA One Server instance, and restore the key on subsequent 2FA One Servers, so that each server maintains the same keys. This procedure should be performed for each subsequent 2FA One Server before any server operation is performed.
