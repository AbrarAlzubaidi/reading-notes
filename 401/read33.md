# What is JSON Web Token?

JSON Web Token **(JWT)** is an open standard **(RFC 7519)** that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret or a public/private key pair using RSA or **ECDSA.**

- JWT can be encrypted to also provide secrecy between parties
- Signed tokens can verify the integrity of the claims contained within it, while encrypted tokens hide those claims from other parties.
- When tokens are signed using public/private key pairs, the signature also certifies that only the party holding the private key is the one that signed it.

## When should you use JSON Web Tokens?

1. Authorization: Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token. Single Sign On is a feature that widely uses JWT nowadays.

2. Information Exchange: JSON Web Tokens are a good way of securely transmitting information between parties. Because JWTs can be signed—for example, using public/private key pairs—you can be sure the senders are who they say they are. Additionally.

## JSON Web Token structure

1. Header: consists of two parts: the type of the token, which is JWT, and the signing algorithm being used, such as HMAC SHA256 or RSA

Ex:

    {
    "alg": "HS256",
    "typ": "JWT"
    }

2. Payload: contains the claims.
**claims** are statements about the user and additional data. type of it 
        -  registered
        - public
        - private claims.

EX:

    {
    "sub": "1234567890",
    "name": "John Doe",
    "admin": true
    }

3. Signature: To create the signature part you have to take the encoded header, the encoded payload, a secret, the algorithm specified in the header, and sign that.

## How do JSON Web Tokens work?
- In authentication, when the user successfully logs in using their credentials, a JSON Web Token will be returned. Since tokens are credentials, great care must be taken to prevent security issues. In general, you should not keep tokens longer than required.

- Whenever the user wants to access a protected route or resource, the user agent should send the JWT, typically in the Authorization header using the Bearer schema.

- **note that with signed tokens, all the information contained within the token is exposed to users or other parties, even though they are unable to change it. This means you should not put secret information within the token.**

## Why should we use JSON Web Tokens?

- As JSON is less verbose than XML, when it is encoded its size is also smaller, making JWT more compact than SAML. This makes JWT a good choice to be passed in HTML and HTTP environments.


------


# Django Runserver Is Not Your Production Server

## A Production Stack
- A production setup usually consists of multiple components, each designed and built to be really good at one specific thing. They are fast, reliable and very focused.
- When a request arrives at your server, it should be passed to a dedicated web server
- The next component is an application server. It gets those fancy requests and uses them to construct Python objects which are usable by Django

## How Does Django Fit In? 

1. Your project provides a uwsgi.py file, which contains a function to be called by the application server. This function gets a Python object representing the incoming request.

2. This function calls your code, and produces a response object which is passed to the WSGI server. There the response is translated into a HTTP response and is passed back to the web server, which finally delivers it to the user.


***resources**

1. [What is JSON Web Token?](https://jwt.io/introduction/)
2. [How to Use JWT Authentication with Django REST Framework](https://simpleisbetterthancomplex.com/tutorial/2018/12/19/how-to-use-jwt-authentication-with-django-rest-framework.html#installation--setup)
3. [Django Runserver Is Not Your Production Server](https://vsupalov.com/django-runserver-in-production/)