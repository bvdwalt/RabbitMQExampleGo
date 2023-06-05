# RabbitMQExampleGo
An example app using RabbitMQ in Go

First run RabbitMQ locally using docker:<br>
```docker run -d --hostname my-rabbit --name RabbitMQExampleGo -e RABBITMQ_DEFAULT_USER=guest -e RABBITMQ_DEFAULT_PASS=guest -p 15672:15672 -p 5671:5671 -p 5672:5672 -p 15671:15671 -p 25672:25672 rabbitmq:3-management```

Run the two go programs using the following commands:<br>
The Producer:<br>
```go run producer/main.go```<br>
AND the consumer<br>
```go run consumer/main.go```