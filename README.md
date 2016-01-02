# Web Engineering 2015-2016 / Microservices
Please, go to the [Wiki](https://github.com/UNIZAR-30246-WebEngineering/Laboratory-6-microservices/wiki) in order to get the instructions for this assignment.


##1. The two microservices are running and regitered
### Account Microservice
![Account Microservice](https://github.com/asabater94/Laboratory-6-microservices/blob/master/1-AccountService.png?raw=true)
### WebService Microservice
(https://github.com/asabater94/Laboratory-6-microservices/blob/master/2-WebService.png?raw=true)

##2. The service registration service has the two microservices registered
![Registration Microservice](https://github.com/asabater94/Laboratory-6-microservices/blob/master/3-RegistrationService.png?raw=true)

##3. A second account microservice is running in the port 4444 and it is registered
![Account Microservice](https://github.com/asabater94/Laboratory-6-microservices/blob/master/4-AccountService2.png?raw=true)

##4. A brief report describing what happens when you kill the microservice with port 2222.
When you kill the Account Microservice in the port 2222, the WebService MicroService shows 'Connection Refused' errors when you try to do an operation. 
When the WebService realizes the AccountService is down, he ask to RegistrationService to another AccountService in other port. After that you can do operation, again.
