# Lab 8

[Youtube](https://youtu.be/I9lf2idtkz8)

## Investigate what Azure managed services could replace self-hosted MongoDB and RabbitMQ.

        Explain why it’s a good fit (e.g., scaling, backups, availability)

### MongoDB --> CosmoDB

CosmoDB would be the service recommanded to replace MongoDB as it is both a NoSQL storage systems. CosmoDB on the other hand offers better integration within a fully Azure cloud environment as it provides:

- Instantaneous and automatic scaling (in MongoDB you have to manually configure it)
- Managed security and compliance posture
- Continuous backup with on-demand restore

CosmoDB offers more then just these feature as it is a fully managed platform as a service. The AKS solution requires more management and configuration.

### RabbitMQ --> Azure Service Bus

Azure Service Bus would be the service recommanded to replace RabbitMQ as it offers managed queue and messaging system that has inherent message persistence/expiration. Azure Service Bus offers more then just persitence as it is a fully managed platform as a service. The AKS solution requires more management and configuration.
