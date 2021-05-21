# Review, Research, and Discussion

1. What’s the difference between `PUT` and `PATCH`?

    - In a PUT request, the enclosed entity is considered to be a modified version of the resource stored on the origin server, and the client is requesting that the stored version be replaced. When we send a PATCH request, however, we only send the data which we want to update

2. Provide links to 3 services or tools that allow you to “mock” an API for development like `json-server`

   - Nock 
   - Postman
   - Wiremock


2. Compare and contrast SOAP and ReST

| SOAP | REST|
|------|------|
|SOAP stands for Simple Object Access Protocol| REST stands for Representational State Transfer|
|SOAP cannot make use of REST since SOAP is a protocol and REST is an architectural pattern.|REST can make use of SOAP as the underlying protocol for web services, because in the end it is just an architectural pattern.|
|SOAP requires more bandwidth for its usage. Since SOAP Messages contain a lot of information inside of it, the amount of data transfer using SOAP is generally a lot. |REST does not need much bandwidth when requests are sent to the server. REST messages mostly just consist of JSON messages. Below is an example of a JSON message passed to a web server. You can see that the size of the message is comparatively smaller to SOAP.|
|SOAP can only work with XML format. As seen from SOAP messages, all data passed is in XML format.|REST permits different data format such as Plain text, HTML, XML, JSON, etc. But the most preferred format for transferring data is JSON|
```jest
SOAP

<?xml version="1.0"?>
<SOAP-ENV:Envelope 
xmlns:SOAP-ENV
="http://www.w3.org/2001/12/soap-envelope" 
SOAP-ENV:encodingStyle
=" http://www.w3.org/2001/12/soap-encoding">
<soap:Body>
 <Demo.guru99WebService
 xmlns="http://tempuri.org/">
   <EmployeeID>int</EmployeeID>
   </Demo.guru99WebService>
 </soap:Body>
</SOAP-ENV:Envelope>
```   
```jest
REST
{"city":"Mumbai","state":"Maharastra"}
```
