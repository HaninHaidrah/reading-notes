# Readings: Event Driven Architecture

## Review, Research, and Discussion
1. What’s the difference between a FIFO and a standard queue?
    * Standard queues guarantee that a message is delivered at least once and duplicates can be introduced into the queue. FIFO queues ensure a message is delivered exactly once and remains available until a consumer processes and deletes it; duplicates are not introduced into the queue.
2. How can the server be assured a message was properly received?
    * once its saved to queue and has been deleted
3. What classic design pattern is best represented by event driven programming?
    - singleton
4. How do you test an event driven system?
    - by testing the trrigers


  ## DOCUMENTATION:
FIFO Queue
:  In FIFO queues, messages are ordered based on message group ID. If multiple hosts (or different threads on the same host) send messages with the same message group ID to a FIFO queue,

Pub/Sub  
:  Publish/subscribe messaging, or pub/sub messaging, is a form of asynchronous service-to-service communication used in serverless and microservices architectures. In a pub/sub model, any message published to a topic is immediately received by all of the subscribers to the topic


## Preview
1. Which 3 things had you heard about previously and now have better clarity on?
    - the queue messages and why to use them
    - how to use msg queues in order to save messages.
    - how to create app using socket.io
2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
   - using aws
   - why to use it
   - how to use it


***AWS*** => SNS is a publisher subscriber network, where subscribers can subscribe to topics and will receive messages whenever a publisher publishes to that topic. AWS SQS is a queue service, which stores messages in a queue
NS is a distributed publish-subscribe system. Messages are pushed to subscribers as and when they are sent by publishers to SNS.
SNS supports several end points such as email, sms, http end point and SQS. If you want unknown number and type of subscribers to receive messages, you need SNS.
With Amazon SNS, you can send push notifications to Apple, Google, Fire OS, and Windows devices , as well as to Android devices in China with Baidu Cloud Push. You can use SNS to send SMS messages to mobile device users in the US or to email recipients worldwide.

![img](https://miro.medium.com/max/628/1*mdUPKzrfJFuXa4d43KhKUQ.png)