# Rest

## REST Architectural Style
The REST architectural style was documented by Roy Fielding in his dissertation in the year 2000 in an effort to provide a documented architecture that could be used to guide the development and design of the modern web. The first part of this paper characterised a large number of existing architectural constraints of which the ones covered above are only a subset.

In the second part of the paper REST is defined by composing a number of these architectural constraints into a cohesive whole. The patterns used are:
 1. **Client Server:** This constraint provides separation of concerns, improves scalability and improves the portability of the interface.
 2. **Stateless:** This constraint requires that each request contains sufficient state for the server to understand what to do... this provides visibility, readability and scalability.
 3. **Cacheable:** This constraint requires that all responses from the service to its clients are explicitly labelled as cacheable or non-cacheable so that intermediary servers or components can cache responses. This improves efficiency, scalability and user-perceived performance.
 4. **Uniform Interface:** This constraint defines a simple standard for working with a REST service. It includes identification of resources by URI, manipulation of resources through representation, self-descriptive message and HATEOAS.
 5. **Layered System:** This constraint requires that a client should not be able to tell if it is connected to the end server or to an intermediary. Layered systems cause a reduction in performance, but this should be counteracted by caching.
 6. **Code On Demand (optional):** This optional constraint allows client functionality to be extended by downloading and executing code from the server.
