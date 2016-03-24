# Troubleshooting 2FA ONE: Error Logging

Error Logging is available in 2FA One Server to aid in Level 2 and Level 3 support request resolution by 2FA. Error logging is initiated on 2FA One Server’s web and service sites through modifications to web.config files. Once enabled, error events within 2FA One Server are sent to log files that are provided to 2FA’s support team for detailed analysis and issue resolution.

To enable error logging do the following:

1.	Run Notepad.exe as an Administrator by right clicking on the application and selecting Run
		as administrator.
2.	Within Notepad, click File\Open and browse to the following:
<Drive>Program Files\2FA\ONE Server\ServerSite
3.	Select All Files from the drop down box next to the File Name drop down.
4.	Select the web.config file and click Open.
5.	The web (web.config) file will open in Notepad. Copy the diagnostic configuration listed
		Below this step. Scroll all the way to the bottom of the file and position the
		cursor to the left of “</configuration>”, right click, select Paste (the diagnostic information
		will appear), and press enter. 

	<system.diagnostics>
<sources>
<source name="ONE" switchValue="All">
<listeners>
<add name="2FAOneLog" traceOutputOptions="ProcessId,ThreadId,DateTime" initializeData="2FAOneLog.log" type="System.Diagnostics.TextWriterTraceListener" /> </listeners>
</source>
</sources>
<trace autoflush="true" /> </system.diagnostics>

**Note:**	Performing a cut and paste action between PDF and a text file commonly loses the formatting of quotation marks. You may need to perform a find and replace on all your quotation marks or logging will not function.

6.	Click File and click the Save option.
7.	Click File\Open and browse to the following:
<Drive>Program Files\2FA\ONE Server\Website
8.	Select All Files from the drop down box next to the File Name drop down.
9.	Select the web.config file and click Open.
10.	Repeat steps 5 & 6.
11.	Reproduce the error experienced on the 2FA One Server. Once reproduced a log file
named 2FAOneLog will appear in the servicesite and website folders. Send the
2FAOneLog file to 2FA support.

**Note:**	As soon as the issue is resolved you should revert the changes made in both web (web. config) files. Failure to do so will result in performance degradation.
