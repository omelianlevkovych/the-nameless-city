# Introduction
In this RMQ folder I am going to play with the Rabbit Message Queue a bit.

# jargon
* _producing_ means sending. A program that send messages is a _producer_.
* a _queue_ is a name for post box which lives inside RMQ. Although messages can only
be stored inside a _queue_. A queue is only bound by the host's memory & disk limits, it's
essentially a large message buffer. Many _producers_ can send messages that got to one queue,
and many _consumers_ can try to receive data from one _queue_.
* _consuming_ has a similar meaning to receiving. A _consumer_ is a program that mostly waits
to receive messages.

Note that producer, consumer, and broker do not have to reside on the same host; indeed in most
applicaitons they don't.  
An applicaiton can be both a producer and consumer.


# configuration
Creating a queue (in Startup) is idempotent; it will only be created if it doesn't exist already.


# CLI
https://www.rabbitmq.com/cli.html  
Open the shell in the container (on windows: docker desktop -> CLI) and type the command, for instance:
```sh
rabbitmq-diagnostics cluster_status
```

# RMQ elements
## Exchange
Messages are not published directly to a queue. Instead, the producer sends messages to exchange.  
An exchange is responsible for routing the messages to different queues with the help of header
attributes, bindings, and routing keys.  
**Binding** is a 'link' to bind exchange and a queue.