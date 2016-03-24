# Question & Answer Method

The Question & Answer sub-menu enables you to establish, configure, enable, and maintain Q&A so that users can authenticate to a system using previously-established Emergency Access, user-selected or administrator defined questions. 

This is also often referred to as Knowledge-Based Authentication.

Within the Question & Answer submenu, there are five submenus:

1.	**Profile List:** Provides an overview of the configured Q&A Profiles. Available configurations include:
  2.	**Emergency Access:** Use this profile in conjunction with 2FA ONE Client to enable Emergency Access and Secure Workflows in 2FA ONE Server. The questions in this list are hard coded and cannot be changed due to the static nature of 2FA ONE Client’s question set.
  3.	**Secure Workflow Admin:** Use this profile if you would like to create custom question sets within 2FA ONE Server for Secure Workflows.
  4.	**Secure Workflow User:** Use this profile if you would like users to create their own questions to answer for use within 2FA ONE Server for Secure Workflows.
5.	**Policies:** Provides the ability for organizations to establish Q&A policies.
6.	**Question Sets:** Provides the ability to create, modify and delete question sets that are assigned to Q&A profiles.
7.	**New Profile:** Provides the ability for organizations to create custom profiles that can then be paired with Authentication Sets and assigned to users.
8.	**New Policy:** Provides the ability to create custom Q&A policy beyond that delivered by default with 2FA ONE Server.
  9.	**Note:** Once a user has been assigned to a Question Set the Set cannot be deleted or modified.


### Profile List

This is the default submenu and provides an overview of the defined Q&A configurations. From this submenu, you can edit or delete previously configured Q&A profiles. 

By default, the Emergency Access question set is defined containing 27 commonly-used secret questions. 

These questions are used for Emergency Access and Secure Workflows. 

You cannot edit or change these questions due to the requirement for these questions to be present in 2FA ONE Client. 

You may edit the default Administrator Defined Question list which contains ten pre-defined questions or you may make a new list all together.

2FA ONE Server provides organizations with the flexibility to:

1.	Increase the number of user-defined questions
2.	Establish administrator-defined questions,
3.	Create an M of N structure that requires users to answer a defined number of previously-enrolled questions, such as three of five, and
4.	Create policy that defines the length of answers users must provide and whether the user may repeat answers within the same answer set.

### Policies & Question Sets

Question and Answer Policy is used to set a number of variables, including:

* The number of questions the user must select (or provide in the case of user defined) during enrollment.
* The number of questions the user will be challenged with during routine challenges such as Emergency Access and Secure Workflows. In all cases, the user is required to answer all questions correctly. There is no margin of error in 2FA ONE Server Question and Answer logic. However, user answers are case insensitive, and spacing is removed, in order to reduce the likelihood of common errors in typing.
* The minimum number of characters that must be present in each answer. This feature addresses the problem with users answering single letter answers to all their questions. 
* The requirement for all answers to be unique. This feature addresses the problem with users answering the same answer to every question.


The Question and Answer Policy submenu provides the ability for organizations to create custom Q&A policies and edit out-of-the-box policies. 

By default there are two Q&A policies with varying degrees of security from High to Low. The default Policy contains a policy based upon best practices. 

Q&A policies can be edited or you can create your own Q&A policy by click on the New Policy link. Q&A policy is assigned to a Profile that can be assigned to a Set; then, the Set can be assigned to a user.

**Note:**	If you create new questions within the admin portal. Those questions will not be available for your users to register with. 

Currently in order to utilize custom questions, you will need to contact us so we may create a custom template that will be import into your SQL database by us. 

Most of our customers find that the 27 default questions we provide are sufficient for their environment.

### New Profile

In order to assign a new Profile to a Set you must first create the new Profile. To create a new Profile, click the New Profile link and the New Q&A Profile pop-up will appear. 

Enter a Name and Description for the new profile, select the desired question set and Q&A Policy. 

Once you have made your desired selection, click the Add button.

### New Policy

In order to assign a new Policy to a Profile you must first create the new Q&A Policy. To create a new Q&A Policy, click the New Policy link, and the Create Question and Answer Policy pop-up will appear. 

You must name the new policy and select your desired settings.

* **Required Answers:** This number represents how many question must be enrolled.
* **Required Correct:** This number represents how many correct answers are needed.Minimum Answer Length:	This number represents how short the answer can be.
* **Require Unique Answers:**	Determines if you can have the same answer for multiple questions

