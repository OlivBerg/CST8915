# Lab 2

[Lab 2 demo Olivie Bergeron - CST8915 Full-stack Cloud-native Development - YouTube](https://youtu.be/J5BJiYg7N3c)

[Store Front](https://github.com/OlivBerg/store-front)

[Order Service](https://github.com/OlivBerg/order-service)

[Product Service](https://github.com/OlivBerg/product-service)

FYI, I did not commit any of the .env file because its bad practice. That is why you do not see them in my repos.

#### What changes did you make to the order-service and product-service to comply with the Configurations and Backing Services factors of the 12-Factor App methodology?

We Stored the configs (.env) files in the local setup for each service and for the backing services we created a vm for only the message manager RabbitMQ. We then connected the order-service to RabbitMQ to Product-Services via an API which the creds are stored in a .env file.

[Resourced used](https://12factor.net/)

#### Why is it important to use environment variables instead of hard-coding configurations in your application?

Enhances security by preventing sensitive information exposure.

#### Why is it important to have separate repositories for each microservice? How does this help maintain independence and scalability of each service?

Services are designed for independence and autonomy, enabling independent scaling, updating, and deployment.
