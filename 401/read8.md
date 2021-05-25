# Access Control (ACL)
## Review, Research, and Discussion
* When is Basic Authorization used vs. Bearer Authorization? 
  * The Basic authentication schemes are dedicated to the authentication using a username and a secret.

  * The Bearer authentication scheme is dedicated to the authentication using a token even if this scheme comes from an OAuth2 specification, you can still use it in any other context where tokens are exchange between a client and a server.
  

* What does the JSON Web Token package do?
  *  used to send information that can be verified and trusted by means of a digital signature.


* What considerations should we make when creating and storing a SECRET?
  * Use encryption to store secrets within .git repositories.
  * Use environment variables.
  * Use "Secrets as a service" solutions.

## Vocabulary Terms

### encryption :
*  securing data by encoding it mathematically . 
### token :
* 	is a  secure format used to transmit sensitive information between two services .
### bearer :
*  is an HTTP authentication scheme originally created as part of OAuth 2.0, but is now used on its own.
### secret :
* a key that is added when generating the token as part of it to scure it more.

### JSON Web Token :
* A token used for authentication, consists of a header, a payload and a signature. 


# Role-based access control

![](https://www.dnsstuff.com/wp-content/uploads/2019/10/role-based-access-control.jpg)

***Role-based access control*** is an approach to restricting system access to authorized users. It is used by the majority of enterprises with more than 500 employees, and can implement mandatory access control (MAC) or discretionary access control (DAC).

Role-based access control (RBAC) is a policy-neutral access-control mechanism defined around roles and privileges. The components of RBAC such as role-permissions, user-role and role-role relationships make it simple to perform user assignments. A study by NIST has demonstrated that RBAC addresses many needs of commercial and government organizations. RBAC can be used to facilitate administration of security in large organizations with hundreds of users and thousands of permissions. Although RBAC is different from MAC and DAC access control frameworks, it can enforce these policies without any complication.

## RBAC vs. ABAC vs. ACL
There are some alternatives for/variations of RBAC, including:

1. Access control lists (ACL) — An ACL is a means of defining access rights by a given user or user group, to a specific object, such as a document.  As a simple example, an ACL could be used to allow users from one department to make changes to a document, while only allowing users from other departments to read the document.

1. Attribute-based access control (ABAC) — ABAC, sometimes known as policy-based access control, can use a variety of attributes, including user department, time of day, location of access, type of access required, etc. to determine whether a user’s access request should be granted.

### RBAC implementation:
* Inventory your systems
* Analyze your workforce and create roles
* Assign people to roles
* Never make one-off changes
*  Audit