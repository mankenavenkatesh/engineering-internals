# Why Sessions?

- let's a user is logged into a e-commerce website by entering password and username.
-  Server verified the credentials, and user is logged in.
- Now  when he navigates to any other page (billing page, cart page), he has to login again for server to know who the user is. 
- this can be solved using Sessions.


## Session
Instead of typing username and password for every single page, if browser can remember who the user is....and request page from server using the remember credentials...... 
 (that's the idea behind sessions.)

How it works?
- when user sends login credentials for first time, server will validate the credentials.
- Upon validation, server will create a session object. 


 ## Cookie
 How browser remembers?
 - via cookies
 - cookies are nothing but strings passed in a request.


 ## Work flow
 - when user logins, the server will tell browser to store information about the user in a `cookie`.
 - From now on, when this user makes request to server, Browser will send `cookie` in the request header.
 - ```
    Example: 
    {
        "User-Agent":"cURL/1.2.3",
        "Accept":"*/*",
        "Host":"localhost:3000",
        "Cookie" : "session = 12345"
    }
- 

## What information about user is stored in cookie
- It cannot be userID. as userID can be easily guessed by hackers.
- Better to send random value. Let's call it SESSION-ID. so, once user logins, server will create a sessionID mapped with user details (userID). This mapping is stored on server. and SessionID is sent in the response
- Cookie will store the sessionID. and in consequent request, SessionID will be sent in http Header.
- Server will check the mapped userID for received sessionID, and processes the request.
- Sessions use cookies to save session ids on the client side, and save all other information on the server side.

## Examples
```

https://astaxie.gitbooks.io/build-web-application-with-golang/en/06.2.html
```


 ## References
 - https://www.youtube.com/watch?v=j8Yxff6L_po




