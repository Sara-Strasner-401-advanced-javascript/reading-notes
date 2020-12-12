# Bearer Authorization

## Review, Research, and Discussion

### Write the following steps in the correct order:
1. Register your application to get a client_id and client_secret
1. Ask the client if they want to sign in via a third party
1. Redirect to a third party authentication endpoint
1. Make a request to a third-party API endpoint
1. Receive authorization code
1. Make a request to the access token endpoint
1. Receive access token

#
1. What can you do with an authorization code?
The authorization code is a temporary code that the client will exchange for an access token. from [Authorization Code Grant](https://www.oauth.com/oauth2-servers/server-side-apps/authorization-code/#:~:text=The%20authorization%20code%20is%20a,approve%20or%20deny%20the%20request.)
1. What can you do with an access token?
Access tokens are the thing that applications use to make API requests on behalf of a user. The access token represents the authorization of a specific application to access specific parts of a user's data. from [Access Tokens](https://www.oauth.com/oauth2-servers/access-tokens/)
1. What’s a benefit of using OAuth instead of your own basic authentication?
In basic authentication, the entirety of the username and password are passed in on each request. In OAuth, the user's information is protected with an access token.


## Document the following Vocabulary Terms

- Client ID- The client_id is a public identifier for apps. from [The Client ID and Secret](https://www.oauth.com/oauth2-servers/client-registration/client-id-secret/)
- Client Secret- The client_secret is a secret known only to the application and the authorization server from [The Client ID and Secret](https://www.oauth.com/oauth2-servers/client-registration/client-id-secret/)
- Authentication Endpoint- the endpoint on the authorization server where the resource owner logs in, and grants authorization to the client application [from OAuth 2.0 Endpoints](http://tutorials.jenkov.com/oauth2/endpoints.html)
- Access Token Endpoint - where apps make a request to get an access token for a user
- API Endpoint- the location from which APIs can access the resources they need to carry out their function. 
- Authorization Code- The authorization code is a temporary code that the client will exchange for an access token.
- Access Token- Access tokens are the thing that applications use to make API requests on behalf of a user.

## Preview
1. Which 3 things had you heard about previously and now have better clarity on?
- APIs, RESTful practices, linked lists
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
- the OAuth workflow/steps, Big O, OAuth vs basic authentication
1. What are you most excited about trying to implement or see how it works?
- integrating Google authorization
