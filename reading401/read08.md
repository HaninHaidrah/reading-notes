# Reading: Access Control (ACL)

## Review, Research, and Discussion
1. When is Basic Authorization used vs. Bearer Authorization?
  - basic used when the user sign in kind of authuntication ,while bearer to check if the user valid or has the permission to do .
2. What does the JSON Web Token package do?
  - it creates and verifies the token for the user.
3. What considerations should we make when creating and storing a SECRET?
  - should be more complicated.

## DOCUMENTATION
encryption
:  its a method to protect the sensitive data by encoded it
token
:  its a proxy to void user save his data on the browser.
bearer
:  its a level of security that used to check the user validatation and available actions to do in the app by checking and verifying the token
secret
:  its a signeture used once the client create and verify tokens
JSON Web Token
:  it's a package used to create tokens

## PREVIEW
Which 3 things had you heard about previously and now have better clarity on?
 - Bearer auth
 - tokens
 - how to identify the actions related to user type.
Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  - Whats RBAC
  - DIIFERENCE BETWEEN Acl and abac
What are you most excited about trying to implement or see how it works?
  - see how the security will be .


* ***RBAC*** =>  is nothing more than the idea of assigning system access to users based on their role within an organization. The system needs of a given workforce are analyzed, with users grouped into roles based on common job responsibilities and system access needs. Access is then assigned to each person based strictly on their role assignment. With tight adherence to access requirements established for each role, access management becomes much easier.

* ***Attribute-based access control (ABAC)*** — ABAC, sometimes known as policy-based access control, can use a variety of attributes, including user department, time of day, location of access, type of access required, etc. to determine whether a user’s access request should be granted.

![img](https://www.dnsstuff.com/wp-content/uploads/2019/10/role-based-access-control.jpg)