# Bulk Import Users

Bulk Import Users enables you to import multiple users simultaneously using a CSV file, or by selecting an OU or group. To use the Bulk Import Users option:
Select the Users>New Users>Bulk Import Users submenu.


### To Import from CSV:
* Enter the location of a CSV file on the Bulk Import Users page to load, or click Browse to navigate to the file.
* Click the Ignore First Line check box if required. This would be in case the first line of the CSV file contains generic information such as column headers, which is common in most auto-generated CSV files.
* Click Import Users to complete the task.
  * Note: The CSV files must contain the following information in the specified order. You may leave a field blank if you do not wish to set that or if you would like it set to the default.
    * User name, Domain, Email, Language, AuthSet, Role
    * For example:
      * TestUser1,2FA,TestUser1@2FA.com,English,Smart Card Only,User
      * TestUser2,2FA,TestUser2@2FA.com,German,ContactlessOnly,Admin


### To Import by OU:
* Type in the OU's Distinguished Name or click the icon to launch the Lookup Tool.
* Select the desired default Authentication Set and Role from the dropdown at the bottom.
* Click Import Users button to immediately import all users of that OU.


### To Import by Group:
* Type in the Group's Distinguished Name or click the icon to launch the Lookup Tool
* Select the desired default Authentication Set and Role from the dropdown at the bottom. 
* Click Import Users button to immediately import all users of that Group

