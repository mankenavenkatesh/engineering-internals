# Authentication
User authentication is the verification of an active human-to-machine transfer of credentials required for confirmation of a user’s authenticity;

- In simple words, verify user credentials to confirm user authenticity. 

## How to Authenticate user?
- Traditionally, user authentication has typically consisted of a simple ID and password combination. Increasingly, however, more authentication factors are added to improve the security of communications.

## Authentication factors
The main authentication factors are knowledge, possession and inherence:

- `Knowledge` factors include all things a user must know in order to log in, User names or ID password and pin numbers all fall under this category.
- `Possession` factors consist of anything a user must have in their possession in order to log in; this category includes one-time password tokens as key fobs or smartphone apps, employee ID cards and SIM card-based mobile phones.
- `Inherence` factors include any inherent traits the user has that are confirmed for login; this category includes the scope of biometrics: retina scans, iris scans, fingerprint scans, finger vein scans, facial recognition, voice recognition, hand geometry and even earlobe geometry.
- `User location` is sometimes considered a fourth factor for authentication. The ubiquity of smartphones can help ease the burden here: Most smartphones are equipped with GPS, enabling reasonable surety confirmation of the login location. Lower surety measures include the MAC address of the login point or physical presence verifications through cards and other possession factor elements.


## 2FA, 4FA
```
The use of at least one-factor of each of these four-factor types is considered four-factor authentication (4FA).
```

 Selecting four authentication factors out of two categories is only two-factor authentication (2FA) and, as such, less likely to add significantly to the security of the procedure.



Web applications need robust authentication and authorization mechanisms. 
This repo explains most common authentication methods in web application development

## Authentication Mechanisms 
- [stateless-authentication-with-json-web-tokens](https://github.com/mankenavenkatesh/webapp-internals/blob/master/Authentication/stateless-authentication-with-json-web-tokens)

- https://searchsecurity.techtarget.com/definition/user-authentication#:~:text=User%20authentication%20is%20the%20verification,do%20not%20require%20user%20input.