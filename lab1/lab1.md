# Lab 1

[Lab 1 demo Olivie Bergeron - CST8915 Full-stack Cloud-native Development - YouTube](https://youtu.be/bhErF2gC8fk)

### **Order Service (Node.js)**
Order services is a pretty simple Node service that provides one route, Post ('/oders').  This service is in charge of facilitating the queue order from the client to RABBITMQ. The service is handled with the help NodeJS a mainly server side JavaScript environement. 

This service initialization of CORS functions which enables Node to to accept data from all routes. TLDR, it enable the service to talk (allows requests) with other services/platforms like our frontend for instance. The post route works by listening for a request made by the clients to create an order queue. The route accepts the request  &rarr; connect to RABBITMQ &rarr; create a channel with RABBITMQ &rarr; define the queue and convert order &rarr;  assert and send to queue &rarr; Sends client a response "Order Received". As well, in a node application, its important to have the application be listening to the port wanted otherwise the no communication will be made. 

### **Product Service (Rust)**
Product Service is again a pretty simple Rust server application that provides a routing service to 'Get' the products for sale. These products are then displayed to the client/front-end for the user to experience.  

This service makes use of  Warp  which is [a super-easy, composable, web server framework for warp speeds](https://docs.rs/warp/latest/warp/). This framework enable the service 'product' route. Client first makes a 'Get' request to gain access to some information (products info that are hard coded), and sends them back to the client. Just like the Order Service, the Product Service listens to incoming request through a specific port. 

### **Store Front (Vue.js)** 

The Store Front is build in Vue.js a JavaScript framework made be lightweight. This page offers a pretty basic approach to a storefront. Vue.js is designed to follow the '[SinglePage Application](https://developer.mozilla.org/en-US/docs/Glossary/SPA)' approach, meaning the application will only load one page/file, allowing the body of that file to be updated. In our application we see just that through the help of our JavaScript fetch request made in our script element. In the '<script/>'  element we see two fetch requests. The first one is the 'fetchProducts()' that sends a get request to obtain the product info and awaits a response. And the last one is the 'SubmitOrder()' that sends a post request to make a queue order for the product the user wants to purchase. 


