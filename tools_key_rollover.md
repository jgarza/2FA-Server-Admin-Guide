# KEY ROLLOVER TOOL

Key Rollover is a means to change the cryptographic keys associated with 2FA One. This is provided in the event that you believe your keys are compromised or to adhere to more stringent compliance requirements that may expect cryptographic material be changed on a routine basis.

**Note:**	Extreme care must be taken before performing the following tasks. Failure to complete all required steps could result in a catastrophic, unrecoverable failure your deployed 2FA ONE infrastructure. It is suggested that you back up your original keys, as described in the previous section before attempting any Key Rollover.

The utility to perform Key Rollover is located within the Tools folder of your 2FA One Server installation directory: <INSTALLDIR>\2FA\One Server\Tools\KeyRollover.

### Performing Key Rollover

Prior to starting the key rollover process you must perform three prerequisite steps:

1. **Stop IIS:** Manually perform this step through IIS Console.
2. **Backup Database:**	backup the 2FA ONE Database.
3. **Backup Server Key:** be sure to 'right-click & run as administrator'

Once complete, open the 2FA ONE Server Key Rollover utility and manually verify that you have Completed. Each of the three tasks described above by check marking each checkbox associated with each task. 

Once All tasks have been checked the Start button will become enabled.

Click the Start button and the Key Rollover Process will start. Once completed you will be notified that the key rollver process completed successfully.

Restart IIS and the process is complete.
