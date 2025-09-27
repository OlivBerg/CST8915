# Lab 3
[Youtube](https://youtu.be/dF431-bwnwc)

[Order Service](https://github.com/OlivBerg/order-service)

[Product Service](https://github.com/OlivBerg/product-service-rebuild)

[Store Front](https://github.com/OlivBerg/store-front)

## Reflection Questions

### What challenges did you encounter when configuring environment variables in the GitHub Actions workflow?
I accidently misspelled a port number. The build never reported an error which it makes sense for this type of error. To fix this issue I had to look that he Azure logs of the respected Web App. From there, I found that the container could not open a port for "3-3-". Hit my head then proceeded to fix the issue.

### How does deploying microservices on Azure Web App Service differ from running them locally?
Its pretty similar, the only difference is where the user need to setup the environment variables. On Azure, we need to go the environment page, and enter them there and the managed service will create its own .env file for your app. Locally, you need to create a .env file yourself. 

### Why is it important to use environment variables for configurations in a cloud environment?

There is serveral reason why its important. To name a few, seperation of config/env from code is crucial for ease of use, best coding practice and security (sensitive keys should not be exposed, being hardcoded in the source code is exposing it). In the cloud, the main way to share config in a containerized system is through environment variables which aligns with the third factor Configs of the 12 factors.