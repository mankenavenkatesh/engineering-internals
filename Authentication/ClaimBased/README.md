# Claim based Authentication
## Problem Statement (Single Sign-on)
A „classical authentication” approach means that every application has its own authentication mechanism that leads to many different problems. There are lots of ways to build identity support into an application, and each communication framework treats identity differently, with different object or storage models. One of the most important problems of this approach is dispersion of the user identity. Each application stores its own copy of user data, which is used to build user identity. Very often user data (identities) are duplicated in multiple applications or systems, generating problem of data integrity. This kind of approach to authentication does not support Single Sign On (SSO) mechanism. Nowadays, mechanism called SSO is becoming more and more popular due to possibility for allowing authentication in many applications using one application of user identity. User logs once (authenticates and authorizes) and gains access to all systems without being prompted to log in again. Using Active Directory (and authentication based on AD) partially solved problem with SSO. Despite its advantages AD approach cannot be used in every situation.


## Solution
One step toward to solve those problems is to stop building custom identity plumbing and user account databases into every new application. Claims-based identity is a straightforward idea, founded on a limited number of concepts: claims, tokens, identity providers, and a few more. This approach helps us to reduce the excess of identity management by providing a central point for user and role administration (providers support for Single Sign On mechanism).


Claims-based authentication is more general authentication mechanism that allows users to authenticate on external systems that provide asking system with claims about user. 

## What does a claim contain?
- Claims can contain information about the user, roles or permissions, useful to build flexible authorization model. Token contains one or more claims and every claim contains some specific information. The token is digitally signed by token issuer when it’s created, so that it can be verified at the receiver end. Token can also contain additional information e.g. expiry date or id.


### References
- https://kariera.future-processing.pl/blog/introduction-to-claims-based-authentication-and-authorization-in-net/
- https://www.youtube.com/watch?v=SWiHo3tFlQs