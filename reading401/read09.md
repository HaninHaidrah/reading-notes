# Reading: Authorization/Authentication
## Review, Research, and Discussion
1. What header(s) are used in authentication and authorization
    - The headers hold the encrypted password and it will be used to decode the password again
2. What is safe to put into a JWT
   - it will save the sensentive data for the user like paaword when he goes through the pages
3. How are JWTs validated
   - there are two methods to create a token then verify the first one is **sign** the next is **verify** and both use Sercert 

## DOCUMENTATION 

RBAC
:  Role-based access control (RBAC) is a method of restricting network access based on the roles of individual users within an enterprise. RBAC ensures employees access only information they need to do their jobs and prevents them from accessing information that doesn't pertain to them.

User Roles
:  A permission is the right to access one or more system objects. A role is a group of permissions. Roles can be assigned to any user or user group, and a user or user group can have more than one role. Unlike hierarchical users, a role does not contain another role.

JWT Token
:  JSON Web Token (JWT) is a JSON encoded representation of a claim(s) that can be transferred between two parties. The claim is digitally signed by the issuer of the token, and the party receiving this token can later use this digital signature to prove the ownership on the claim


## Illustrations:

- Jwt=> ![jwt](https://www.vaadata.com/blog/wp-content/uploads/2016/12/JWT_tokens_EN.png)
- RBAC => ![PBAC](https://www.dnsstuff.com/wp-content/uploads/2019/10/role-based-access-control.jpg)

## Preview
1. Which 3 things had you heard about previously and now have better clarity on?
  - The main concept of User Roles
  - How to give permession to each Role
  - What's the idea behind get()and sign()
2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  - more about jwt library
  - other levels od security
3. What are you most excited about trying to implement or see how it works
  - adding more implments to the backend.