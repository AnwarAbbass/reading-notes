#  Event Driven Architecture
## Review, Research, and Discussion
* What’s the difference between a FIFO and a standard queue?
  * Standard queues guarantee that a message is delivered at least once and duplicates can be introduced into the queue. FIFO queues ensure a message is delivered exactly once and remains available until a consumer processes and deletes it; duplicates are not introduced into the queue.

* How can the server be assured a message was properly received?
  * we can use the socket.io's acknowledgements.


* What classic design pattern is best represented by event driven programming?
  *  Event-driven from end to end.



* How do you test an event driven system?
  *  using Unit Tests.



## Vocabulary Terms

### FIFO Queue :
* first-in, first-out.

### Pub/Sub:
*  is an asynchronous messaging service that decouples services that produce events from services that process events.

## AWS — Difference between **SQS** and **SNS** 

![](https://www.techrepublic.com/a/hub/i/r/2018/08/06/dc16c8f2-3889-48c1-93c4-e1ea2023bc8d/resize/1200x/944114825f9c21e785c2d84a23acbf9b/awscloud.jpg)

* **SNS** is a distributed publish-subscribe system.
* Messages are pushed to subscribers as and when they are sent by publishers to **SNS**.

![](https://miro.medium.com/max/3200/0*wMrZ5wPX3kxqGZjm.png)

* **SQS** is distributed queuing system , Messages are not pushed to receivers, Receivers have to poll or pull messages from SQS.

![](https://miro.medium.com/max/3200/0*gbEjL3cwmpHbYZ7Y)

### Entity Type

* **SQS**: Queue 
* **SNS**: Topic (Pub/Sub system)

### Message consumption

* ***SQS***: Pull Mechanism - Consumers poll and pull messages from ****SQS***
* ***SNS***: Push Mechanism - ***SNS*** Pushes messages to consumers

### Use Case

* ***SQS***: Decoupling two applications and allowing parallel asynchronous processing
* ***SNS***: Fanout - Processing the same message in multiple ways
### Persistence

* ***SQS***: Messages are persisted for some (configurable) duration if no consumer is available (maximum two weeks), so the consumer does not have to be up when messages are added to queue.
* ***SNS***: No persistence. Whichever consumer is present at the time of message arrival gets the message and the message is deleted. If no consumers are available then the message is lost after a few retries.
### Consumer Type

* **SQS**: All the consumers are typically identical and hence process the messages in the exact same way (each message is processed once by one consumer, though in rare cases messages may be resent)
* ***SNS***: The consumers might process the messages in different ways
### Sample applications

* ***SQS***: Jobs framework: The Jobs are submitted to ***SQS*** and the consumers at the other end can process the jobs asynchronously. If the job frequency increases, the number of consumers can simply be increased to achieve better throughput.
* ***SNS***: Image processing. If someone uploads an image to S3 then watermark that image, create a thumbnail and also send a Thank You email. In that case S3 can publish notifications to an ***SNS*** topic with three consumers listening to it. The first one watermarks the image, the second one creates a thumbnail and the third one sends a Thank You email. All of them receive the same message (image URL) and do their processing in parallel.

![](https://res.cloudinary.com/practicaldev/image/fetch/s--0qV6AkDT--/c_imagga_scale,f_auto,fl_progressive,h_900,q_auto,w_1600/https://dw71fyauz7yz9.cloudfront.net/video-upload__c8bc44f83cd41222de8ae55b55c63ef2/thumbs-video-upload__c8bc44f83cd41222de8ae55b55c63ef2-00001.png)

