# Lab 2

[Lab 2 demo Olivie Bergeron - CST8915 Full-stack Cloud-native Development - YouTube](https://youtu.be/J5BJiYg7N3c)

[Store Front](https://github.com/OlivBerg/store-front)

[Order Service](https://github.com/OlivBerg/order-service)

[Product Service](https://github.com/OlivBerg/product-service)

FYI, I did not commit any of the .env file because its bad practice. That is why you do not see them in my repos.

#### What changes did you make to the order-service and product-service to comply with the Configurations and Backing Services factors of the 12-Factor App methodology?

- Codebase #1: One codebase tracked in revision control, many deploys
- Dependencies #2 : Explicitly declare and isolate dependencies
- Config #3 : Store config in the environment
- Backing services #4 : Treat backing services as attached resources

[Resourced used](https://12factor.net/)

#### Why is it important to use environment variables instead of hard-coding configurations in your application?

Enhances security by preventing sensitive information exposure.

#### Why is it important to have separate repositories for each microservice? How does this help maintain independence and scalability of each service?

Services are designed for independence and autonomy, enabling independent scaling, updating, and deployment.
