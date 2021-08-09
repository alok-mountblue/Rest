
# Rest

Representational State Transfer (REST) is an architectural style that defines a set of rules to be used for creating web services. An API is an interface through which one program or web site talks to another. They are used to share data and services. REST API is a way of accessing web services in a simple and flexible way without having any processing. It’s used to fetch or give some information from a web service. All communication done via REST API uses only HTTP request. 

## REST Architectural Style 
There are six architectural constraints :

 1. **Client Server:** This constraint provides separation of concerns, improves scalability and improves the portability of the interface.
 2. **Stateless:** This constraint requires that each request contains sufficient state for the server to understand what to do... this provides visibility, readability and scalability.
 3. **Cacheable:** This constraint requires that all responses from the service to its clients are explicitly labelled as cacheable or non-cacheable so that intermediary servers or components can cache responses. This improves efficiency, scalability and user-perceived performance.
 4. **Uniform Interface:** This constraint defines a simple standard for working with a REST service. It includes identification of resources by URI, manipulation of resources through representation, self-descriptive message and HATEOAS.
 5. **Layered System:** This constraint requires that a client should not be able to tell if it is connected to the end server or to an intermediary. Layered systems cause a reduction in performance, but this should be counteracted by caching.
 6. **Code On Demand (optional):** This optional constraint allows client functionality to be extended by downloading and executing code from the server.

## Working

A request is sent from client to server in the form of web URL as HTTP GET or POST or PUT or DELETE request. After that, a response comes back from server in the form of a resource which can be anything like HTML, XML, Image or JSON. But now JSON is the most popular format being used in Web Services. 

In HTTP there are five methods which are commonly used in a REST based Architecture i.e., POST, GET, PUT, PATCH, and DELETE. These correspond to create, read, update, and delete (or CRUD) operations respectively. There are other methods which are less frequently used like OPTIONS and HEAD. 
Interaction in REST based systems happen through Internet’s Hypertext Transfer Protocol (HTTP).

* GET : The HTTP GET method is used to read (or retrieve) a representation of a resource. In the safe path, GET returns a representation in XML or JSON and an HTTP response code of 200 (OK). In an error case, it most often returns a 404 (NOT FOUND) or 400 (BAD REQUEST). 
 
* POST: The POST verb is most-often utilized to create new resources. In particular, it’s used to create subordinate resources. That is, subordinate to some other (e.g. parent) resource. On successful creation, return HTTP status 201, returning a Location header with a link to the newly-created resource with the 201 HTTP status. 
NOTE: POST is neither safe nor idempotent. 
 
* PUT: It is used for updating the capabilities. However, PUT can also be used to create a resource in the case where the resource ID is chosen by the client instead of by the server. In other words, if the PUT is to a URI that contains the value of a non-existent resource ID. On successful update, return 200 (or 204 if not returning any content in the body) from a PUT. If using PUT for create, return HTTP status 201 on successful creation. PUT is not safe operation but it’s idempotent. 
 
* DELETE: It is used to delete a resource identified by a URI. On successful deletion, return HTTP status 200 (OK) along with a response body. 
 
 ## Response Codes

 Responses from the server contain status codes to alert the client to information about the success of the operation. As a developer, you do not need to know every status code (there are many of them), but you should know the most common ones and how they are used:

 | Status code | Meaning     |
 |-------------|-------------|
 | 200 (OK)    | This is the standard response for successful HTTP requests.|
 | 201 (CREATED)| This is the response for an HTTP request that resulted in an item being created.|
 | 204 (NO CONTENT)|This is the standard response for successful HTTP requests, where nothing is being returned in the response body.|
 | 400 (BAD REQUEST) |	The request cannot be processed because of bad request syntax, excessive size, or another client error.|
 | 403 (FORBIDDEN) |	The client does not have permission to access this resource.|
 | 404 (NOT FOUND) |	The resource could not be found at this time. It is possible it was deleted, or does not exist yet.|








