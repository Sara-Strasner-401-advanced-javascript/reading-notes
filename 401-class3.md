# Express REST API

## Review, Research, and Discussion

1. Name 3 real world use cases where you’d want to change the request with custom middleware
to format the request object, validate names, validate zip codes
1. True or false: The route handler is middleware?
Not necessarily (so truthy?). The distinction is a little blurry in Express. Generally speaking, middleware that examines a bunch of different requests and usually prepares the request for further processing. A route handler that is targeted at a specific URL (or type of URL) and whose main purpose is to send a response back to the client for that URL.
[source](https://stackoverflow.com/questions/58925276/what-is-the-difference-between-a-route-handler-and-middleware-function-in-expres#:~:text=They%20are%20not%20middleware%20functions,the%20only%20one%20callback%20function.)
1. In what ways can a middleware function end the process and send data to the browser?
I'm not quite sure about this one, but I'm thinking it has to do with next().
1. At what point in the request lifecycle can you “inject” middleware?
You can inject middlware any time during the request lifecycle. 
1. What can cause express to error with “Request headers sent twice, cannot start a second response”
I tried researching and couldn't find an answer to this one.

## Document the following Vocabulary Terms

- Middleware - like signposts along the way for the train track of the request object
- Request Object - The Request object is used to get information.
- Response Object - an object or information/data that is sent in response to a request object
- Application Middleware - I read this [Express documenation](https://expressjs.com/en/guide/using-middleware.html#middleware.application) and I'm still not sure what application middleware is.  
- Routing Middleware - middleware that will run for a certain route parameter.
- Test Driven Development- writing tests before writing code, and then writing code specifically designed to pass the given tests
- Behavioral Testing - a software testing method in which the internal structure, design, and implementation of the software being tested is not known to the tester. [source](https://softwaretestingfundamentals.com/black-box-testing/)


## Preview
1. Which 3 things had you heard about previously and now have better clarity on?
ES6 Classes, middlware generally, and req/res objects
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
application middleware, routing middleware, when to use behavioral testing
1. What are you most excited about trying to implement or see how it works?
the Express Router