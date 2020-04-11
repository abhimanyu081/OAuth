# Oauth
## Why OAuth was created?
* Oauth is an specification or protocol that allows a user to grant limited access to their resources
* OAuth is meant for Authorization not for Authentication
* Oauth is meant to authorization between services not for Persons.

### Example
#### Google Photos Service
#### Photo Printing Service 
![](untitled.png)
Connect your photo printing services with Google Photos Services

Using OAuth a user can provide access to thier protected resources to another services without giving credentials of the first service.

Services accessing one another on behalf of the user, OAuth

Current version is OAuth 2.0


Insert Image Here

### Common Analogy
Parking Attendents/Valet
Valet kwy with reduced access
* can not open truck or any compartment
* or ful tank
* only to start and off the engine
Car owner is using 2 services.
1. Car service
2. Valet Service

OAuth
Delegating Access
The OAuth Flow

#### Photo Printing Service OAuth flow

The protected resource server gives the Token just like the Valet key with limited access

OAuth Access Token
Contains user allowed permisions
Trustable - can not be tampered
Token format JWT
The user us already Authenticated, since the user has already logged into both the services he wants to integerate.

## Oauth Key Terms


### 1. Resource (Protected Resources)
This is what other services want to access. Here in example of Google Photos, the Photos on the Google Drive can be the Resource.

### 2. Resource Owner
An entity that is capable of granting access to to protected resource.
The user who has the access of his Google Photos Service is the resource owner of its photos on its google drive.

### 3. Resource Server
The server which is hosting the protected resource.
The Google Drive is the server.

### 4. Client
Client is the app or another service that needs to access the protected resource on behalf of the Resource owner and with resource owner's authorization.

### 4. Authorization Server
The server which issues the access Tokens to the client.

![](oauth-terms.PNG)

In the above interactions, who has the burden of the security?
The person who has the resource.
so its google drive's responsibilty to provide access to the intended and authorized services.

So the resource server is typically coupled with an authorization server also.
To make sure whoever is accessing the resource is authorized.

## Oauth Flows
### 1. Authorization Code Flow

Auth token --> Access token
analogy - room card/key
Best and safest flow in Kaoushik's opinion


Implicit flow







