# Basic Auth
- Basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user and password when making a request. 
- Always sends user/password for authentication
- username/password are `Base64` encoded.

## Why `Base64` Encoding?
- why not send username/password as string???
- to encode non http compatible characters used in username or password into those that are http-compatible.

## Advantages
- As every consequtive request passes username/password, server can easily verify the credentials
- server don't have to manage any state (as it does in session based authetication)
- stateless server
- simple

## Disadvantages
- Non secure as credentials are sent in every request.
- replay attacks. 
- logout is tricky. (Browser caching)


#### References
- https://www.youtube.com/watch?v=501dpx2IjGY
- https://en.wikipedia.org/wiki/Basic_access_authentication