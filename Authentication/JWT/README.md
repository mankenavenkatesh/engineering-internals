# JWT

## why JWT?

### Problems with session ID's 
- Servers store session tokens in cache (in memory) mapped with `user details`. In subsequent request, `sessionID` is passed using which server looks up `cache` and authenticates the user.
- In case of multiple servers, `shared or distributed cache like redis` needs to be used. 
- Problem with `shared cache` is Single point of failure. if `shared cache` goes down, session information is lost.
- To solve this, some use `Sticky Session Pattern` (https://stackoverflow.com/questions/10494431/sticky-and-non-sticky-sessions). 
- But `sticky session pattern` is not scalable. 
- Reference - https://www.youtube.com/watch?v=soGRyl9ztjI


### Alternative model to solve above problems 
- Instead of `Server` storing the data mapped with sessionID, what if on authentication, server creates a `token` with `entire user data`, `sign` using the server publickey and sent back to client. 
- In subsequent request, `token` is passed to server
- `server` fetches `userData` from `token`. 
- For `server` to `trust` the token, server will verify the `signature`
- This is called `JSON Web Token`


### Structure of JWT
- https://www.youtube.com/watch?v=_XbXkVdoG_0

### Examples
- https://jwt.io/introduction/


### Disadvantages of JWT in context of Authorization
- https://www.youtube.com/watch?v=_XbXkVdoG_0