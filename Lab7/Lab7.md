# Lab 7
[Youtube](https://youtu.be/OcNmYdk4Hz8)


## RabbitMQ is a stateless or stateful application
From my understanding, RabbitMQ is a stateful application because it manages and stores data that needs to be persistant across sessions and systems.
## The implications of running RabbitMQ without persistent storage
Running without a persistent storage makes RabbitMQ a weak system as it will loose its storage upon restart, crash or delete. In addition, without a persistent storage it enables the possibility of duplicates.

## What happens when the RabbitMQ pod is deleted or restarted
All queued messages are lost in our scenario.  

## Potential solutions to this problem (research-based)
Implementing a persistent storage solution would be possible solution that can solve this issue. 

## Does using Azure Service Bus solve the issues identified with RabbitMQ Configuration in this Lab?
Yes, Azure Service Bus has a built-in persistent solution that can solve this issue.