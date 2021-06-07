#  AWS: S3 and Lambda
## Review, Research, and Discussion

* Describe “The Cloud”
  * servers that are accessed over the Internet, that run the software and databases  on the servers.

* What is a container (as it relates to computers and servers)?
 * unit of software that packages up code and all its dependencies.


* What is auto-scaling?
  * lets you build scaling plans that automate how groups of different resources respond to changes in demand. 



* What is bandwidth?
  *  is a measure of how much information a network can transfer. 

* How do cloud providers compute service costs?
  * cloud providers determine the expense to maintaining the network. They start by calculating costs for network hardware, network infrastructure maintenance, and labor. These expenses are added together and then divided by the number of rack units a business will need for its IaaS cloud.


## Vocabulary Terms

### Server Instances :
* is a collection of SQL Server databases which are run by a solitary SQL Server service or instance. The details of each server instance can be viewed on the service console which can be web-based or command-line based.

### Containers :
* unit of software that packages up code and all its dependencies .

### Cloud Services :
* are services available via a remote cloud computing server rather than an on-site server. These scalable solutions are managed by a third party and provide users with access to computing services such as analytics or networking via the internet.

### Cloud Architecture :
*  refers to the various components in terms of databases, software capabilities, applications, etc. engineered to leverage the power of cloud resources to solve business problems.

### AWS :
*  Amazon Web Services (AWS) is a secure cloud services platform, offering compute power, database storage, content delivery and other functionality to help businesses scale and grow.

## AWS Lambda

![](data:image/png;base64,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)


* is a serverless computing service provided by Amazon Web Services (AWS).

*  Lambda create functions, self-contained applications written in one of the supported languages and runtimes, and upload them to AWS Lambda, which executes those functions in an efficient and flexible manner.

* **serverless** computing refers to not needing to maintain your own servers to run these functions.
* Use mostly Node JS and Python.
* Lambda is a fully managed service that takes care of all the infrastructure .

* Lambda function runs in its own container.

*  The entire infrastructure layer of AWS Lambda is managed by AWS.

* since the service is fully managed, using AWS Lambda can save you time on operational tasks.

## CDN
* cdn stands for Content Delivery Network (or Content Distribution Network)
![](https://scdn1.plesk.com/wp-content/uploads/2019/04/25141138/image11.jpg)

* a highly-distributed platform of servers that helps minimize delays in loading web page content by reducing the physical distance between the server and the user.


