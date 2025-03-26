# microservices

**Ocean.chat service:** Adapt business logic for request-response protocols (like HTTP, GraphQL, TODO: split some functionalities/routes from the API Gateway to the backend microservices later on).

**Streamer service:** Responsible for maintaining a persistent connection between the frontend and backend, providing functionality for subscriptions (Pub/Sub) and remote procedure calls (RPC). This is implemented by simulating the Meteor DDP protocol.&#x20;

**Watcher service:** Watch change stream of mongodb and broadcast changes to client by streamer service.

**Account service:** Authenticate the user through the streamer service.

**Authorization service:** Provide permission verification function.

<figure><img src=".gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>
