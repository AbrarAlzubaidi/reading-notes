# Status Codes Based On REST Methods

![StatusCodes](https://miro.medium.com/max/920/1*w_iicbG7L3xEQTArjHUS6g.jpeg)

1. **In your own words, describe what each group of status code represents:**

        - 100’s= informational status codes; they usually tell the client that the header part of the request has been           received and the server will try to comply with a             transmission demand of the client.

        - 200’s = the success codes. They tell the client that its request was accepted

        - 300’s = redirection codes. They tell the client that the resource they are requesting isn’t available at the expected location anymore. 

        - 400’s = the client error codes. They are all about invalid requests a client sent to a server.

        - 500’s = the server error codes. Often they indicate problems with overwhelmed servers or unreachable servers behind proxies

2. **What is a status code 202?** 

Accepted - Often used for asynchronous processing. This code tells the client that the request was valid, but its processing will finish sometime in the future

3. **What is a status code 308?**

Permanent Redirect - This tells the client to use another URL to access the resource and not use the current URL anymore. I

4. **What code would you use if an update didn’t return data to a client?**

204

5. **What code would you use if a resource used to exist but no longer does?**

409

6. **What is the ‘Forbidden’ status code?**

the HTTP 403 Forbidden client error status response code indicates that the server understood the request but refuses to authorize it. 