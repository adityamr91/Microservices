# Microservices

**Microservices** - also known as the microservice architecture - is an architectural style that structures an application as a collection of services that are:

- Independently deployable
- Loosely coupled
Services are typically organized around business capabilities. Each service is often owned by a single, small team.

The microservice architecture enables an organization to deliver large, complex applications rapidly, frequently, reliably and sustainably - a necessity for competing and winning in today’s world.

**1. API Gateway:** An API gateway acts as a single entry point for clients to interact with multiple microservices. It handles authentication, routing, load balancing, and other cross-cutting concerns.

**2. Circuit Breaker:** This pattern is used to handle failures and prevent cascading failures in a microservices environment. It involves wrapping remote service calls in a circuit breaker that can open, close, or half-open based on the response from the remote service.

**3. Saga Pattern:** The saga pattern is used to manage long-running transactions across multiple microservices. It involves breaking down a transaction into a series of smaller steps, each with its own compensating action in case of failure.

**4. Database per Service:** In this pattern, each microservice has its own dedicated database. This allows for independent scaling, data isolation, and flexibility in choosing the most appropriate database technology for each microservice.

**5. Event-driven Architecture:** This pattern involves using events to communicate between microservices. Events represent changes in the system and can be used to trigger actions in other microservices, enabling loose coupling and scalability.

**6. Proxy:** A microservice design pattern that can redirect a request to the relevant microservice. It can send the request to several services and combine the outcomes before returning them to the composite or consumer service. Involves creating a proxy service to act as an intermediary for communication between client and target services. The proxy may provide additional functionality, such as security or load balancing. 

**7. Asynchronous Messaging:** A design choice when it comes to microservice communications. In this design pattern, one microservice can publish a message and doesn't need to wait for completion of processing by the consumer to proceed with its work. 

**8. Bulkhead:** The bulkhead pattern involves isolating different parts of a system to prevent failures in one component from affecting others. It helps to improve overall system resilience and fault tolerance.

**10. Service Registry and Discovery:** This pattern involves having a central service registry where microservices can register themselves and discover other services. This helps with dynamic service discovery and allows for flexible scaling and load balancing.
