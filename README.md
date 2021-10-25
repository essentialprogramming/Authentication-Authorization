# Authentication & Authorization

           To know what a user can do, you first need to know who the user is. This is known as **authentication**. It is often done by asking for a set of credentials, such as username & password. Once verified, the client gets information about the identity and access of the user. **Authorization** in system security is the process of giving the user permission to access a specific resource or function. 

![Authorization-vs-Authentication](img/Authorization-vs-Authentication.png)  

            To implement these **Identity and Access Management (IAM)** tasks easily, you can use **OAuth 2.0**, an authorization framework, and OpenID Connect (OIDC), a simple identity layer on top of it.
            
            
            OAuth encapsulates access information in an **access token**. In turn, OpenID Connect encapsulates identity information in an **ID token**. The authentication server can send these two tokens to the client application initiating the process. When the user requests a protected API endpoint, it must send the access token along with the request.
            
![JWT_Simple_Flow](img/JWT_Simple_Flow.png) 

![JWT_Signing](img/JWT_Signing.png) 

## Authentication techniques

1. Password-based authentication

It is the simplest way of authentication. It requires the password for the particular username. If the password matches with the username and both details match the system's database, the user will be successfully authenticated.



2. Passwordless authentication

In this technique, the user doesn't need any password; instead, he gets an OTP (One-time password) or link on his registered mobile number or phone number. It can also be said OTP-based authentication.

3. 2FA/MFA

2FA/MFA or 2-factor authentication/Multi-factor authentication is the higher level of authentication. It requires additional PIN or security questions so that it can authenticate the user.

4. Single Sign-on

Single Sign-on or SSO is a way to enable access to multiple applications with a single set of credentials. It allows the user to sign-in once, and it will automatically be signed in to all other web apps from the same centralized directory.

5. Social Authentication

Social authentication does not require additional security; instead, it verifies the user with the existing credentials for the available social network.

6. Biometrics, such as facial or voice recognition, or fingerprints

##  Authorization Techniques

1. Role-based access control

Role-based access control technique is given to users as per their role or profile in the organization. It can be implemented for system-system or user-to-system.

2. JSON web token


JSON web token or JWT is an open standard used to securely transmit the data between the parties in the form of the JSON object. The users are verified and authorized using the private/public key pair.
