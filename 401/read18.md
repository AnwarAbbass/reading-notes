#  AWS: API, Dynamo and Lambda
## Review, Research, and Discussion

* What are serverless functions?
  * refers to not needing to maintain your own servers to run these functions.


* If you were to create a system that emulated Lambda functions, how would you do it?
  * Lambda function runs in its own container.

  *  The entire infrastructure layer of AWS Lambda is managed by AWS.

  * since the service is fully managed, using AWS Lambda can save you time on operational tasks.

* Describe how a CDN works
  * CDN stores a cached version of its content in multiple geographical locations (a.k.a., points of presence, or PoPs). Each PoP contains a number of caching servers responsible for content delivery to visitors within its proximity.



## Vocabulary Terms

### Serverless Functions :
* refers to not needing to maintain your own servers to run these functions.

### Cloud Storage :
* allows you to save data and files in an off-site location that you access either through the public internet or a dedicated private network connection.


### CDN :
* is a highly-distributed platform of servers that helps minimize delays in loading web page content by reducing the physical distance between the server and the user.




## AWS: API, Dynamo and Lambda

![](https://miro.medium.com/max/636/1*MFvtJPjmug6qbWa92mp5UA.png)


* is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic.

* handles authentication, access control, monitoring, and tracing of API requests.

* replaces the API servers with a managed serverless solution.

* API Gateway sits between the backend services of your API and your API’s users, handling the HTTP requests to your API endpoints and routing them to the correct backends.

![](https://d2908q01vomqb2.cloudfront.net/1b6453892473a467d07372d45eb05abc2031647a/2018/06/13/edge-optimized-1024x513.png)

* API Gateway integrates with many other AWS services like AWS Lambda, AWS SNS, AWS IAM, and Cognito Identity Pools.

## DynamoDB
* is a hosted NoSQL database offered by Amazon Web Services (AWS).

![](https://user-images.githubusercontent.com/54184905/102911788-9709a000-448d-11eb-9161-bac188f78110.png)

* is a key-value and document database that delivers single-digit millisecond performance at any scale. 
*  It's a fully managed, multi-region, multi-active, durable database with built-in security, backup and restore, and in-memory caching for internet-scale applications.

