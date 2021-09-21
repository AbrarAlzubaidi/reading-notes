# What is OAuth

![OAuth](https://i.ytimg.com/vi/CPbvxxslDTU/maxresdefault.jpg)

1. **What is OAuth?**

OAuth, which stands for “Open Authorization,” allows third-party services to exchange your information without you having to give away your password

2. **Give an example of what using OAuth would look like.**

the simplest example of OAuth in action is one website saying “hey, do you want to log into our website with other website's login?” 

3. **How does OAuth work? What are the steps that it takes to authenticate the user?**

oAuth doesn't share password data but instead uses authorization tokens to prove an identity between consumers and service providers

4. **What is OpenID?**

openID allows you to use an existing account to sign in to multiple websites, without needing to create new passwords.



-------------------------------------------------



# Authorization and Authentication flows

![auth](https://images.ctfassets.net/cdy7uua7fh8z/2nbNztohyR7uMcZmnUt0VU/2c017d2a2a2cdd80f097554d33ff72dd/auth-sequence-auth-code.png)


1. **What is the difference between authorization and authentication?**

![dif](https://4.bp.blogspot.com/-AfpUlZHXqNM/UjmEFnh-zbI/AAAAAAAAAh0/_JrUdKFPtao/s1600/Untitled.jpg)

2. **What is Authorization Code Flow?**

authorization code flow is used to obtain an access token to authorize API requests. ... Access tokens while having a limited lifetime, can be renewed with a refresh token.

3. **What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?**

the Authorization Code Flow + PKCE is an OpenId Connect flow specifically designed to authenticate native or mobile application users. 

4. **What is Implicit Flow with Form Post?**

implicit Flow with Form Post flow uses OIDC to implement web sign-in that is very similar to the way SAML and WS-Federation operates. 

5. **What is Client Credentials Flow?**

the Client Credentials flow is a server to server flow. There is no user authentication involved in the process. ... This flow is useful for systems that need to perform API operations when no user is present.

6. **What is Device Authorization Flow?**

the OAuth 2.0 Device Authorization Grant (formerly known as the Device Flow) is an OAuth 2.0 extension that enables devices with no browser or limited input capability to obtain an access token. 

7. **What is Resource Owner Password Flow?**

the Resource Owner Password Credentials flow allows exchanging the username and password of a user for an access token and, optionally, a refresh token. 