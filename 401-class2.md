# Express

## Review, Research, and Discussion

1. What’s the difference between PUT and PATCH?

 PUT only allows a complete replacement of a document. PATCH is used to make changes to part of the resource at a location. 
 [RESTful API Design PUT vs PATCH](https://medium.com/backticks-tildes/restful-api-design-put-vs-patch-4a061aa3ed0b#:~:text=HTTP%20PUT%20method%20only%20allows%20a%20complete%20replacement%20of%20a%20document.&text=HTTP%20resource.&text=A%20PATCH%20request%20on%20the,the%20resource%20%E2%80%94%20changing%20its%20properties.)
1. Provide links to 3 services or tools that allow you to “mock” an API for development like json-server

  - [Mockable.io](https://www.mockable.io/)
  - [Postman](https://www.postman.com/)
  - [Stoplight.io](https://stoplight.io/)

1. Compare and contrast Swagger and APIDoc.js

swagger-ui is for JavaScript web projects that include module bundlers, such as Webpack, Browserify, and Rollup. [Swagger documentation](https://swagger.io/docs/open-source-tools/swagger-ui/usage/installation/)

APIDoc.js apiDoc lets you attach a version number to an API so you can easily track changes between versions. [API Docs](https://apidocjs.com/)


1. Which HTTP status codes should be sent with each type of (un)successful API call?

- 400 Bad Request
- 401 Unauthorized
- 403 Forbidden
- 404 Not Found

- 500 Internal Server Error
- 501 Not Implemented
- 502 Bad Gateway
- 503 Service Unavailable
- 504 Gateway Timeout


1. Compare and contrast SOAP and ReST
SOAP (Simple Object Access Protocol) is a XML-based message protocol, while REST (Representation State Transfer) is an architectural style. SOAP is a more rigid set of messaging patterns than REST. Both SOAP and REST rely on well-established rules that everyone has agreed to abide by in the interest of exchanging information.
[SOAP vs REST. What's the Difference?](https://smartbear.com/blog/test-and-monitor/soap-vs-rest-whats-the-difference/)


1. Document the following Vocabulary Terms
- Web Server - a server is essentially a file. A web server responds to requests made online.
- Express- a library for Node.js, the server uses it to gather information. It lets you specify which functions is called for a certain HTTP verb (get, put, etc.)
- Routing - how an application accesses routes & endpoints and responds 
- WRRC - web request/response cycle. The internet is built on a simple structire of requests and responses.


## Preview
Skim the following materials in preparation for the upcoming lecture. Note the following as you browse the material, and be prepared to participate in discussions during lecture

Which 3 things had you heard about previously and now have better clarity on?
Node, Express, and CI/CD
Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
Supertest, designing tests in general, getting familiar with status codes
What are you most excited about trying to implement or see how it works?
Supertest seems very powerful and applicable to many things. 