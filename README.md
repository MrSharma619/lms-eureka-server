# lms-eureka-server  

i am working on a learning management system-  
teacher posts assignments  
student can do submissions  
teacher can accept or reject those submissions.  

this is the implementation of eureka server  

------------------  

Add eureka discovery client dependency in  
user service,  
task service and  
submission service  

it is already added, you can uncomment it.  

and then add these lines to application.yaml file:  

```
eureka:
  instance:
    prefer-ip-address: true
  client:
    fetch-registry: true
    register-with-eureka: true
    serviceUrl:
      defaultZone: http://localhost:8081/eureka/

```

and then run the server first and then run your microservices.  

now visit  
```
http://localhost:8081
```
  
