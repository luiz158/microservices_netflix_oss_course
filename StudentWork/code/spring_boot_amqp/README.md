


RABBIT MQ:
----------
https://www.rabbitmq.com/tutorials/tutorial-one-spring-amqp.html

Run with Docker image:
---


https://hub.docker.com/_/rabbitmq/

`docker logs ms-rabbit`

**BROKER ONLY:**

`docker run -d --rm --hostname mfk --name ms-rabbit -p 5672:5672 rabbitmq`

**BROKER and ADMIN**
`docker run -d --rm --hostname mfk --name ms-rabbit -p 5672:5672 -p 15672:15672 rabbitmq:management`

**View RabbitMQ Status**

`docker exec ms-rabbit rabbitmqctl status`

**ADMIN URL:**

[http://localhost:15672](http://localhost:15672)


