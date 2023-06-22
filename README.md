# python-microservices-with-rabbitmq

### this project is based on this tutorial:
https://www.youtube.com/watch?v=ddrucr_aAzA

### this video is about 2 module: "product" and "main"
### "main" is like a client side where it will list the products and client can give it a "like", this service is by django
### "product" is like a admin side where admin can do CRUD for the products, this service is by flask
### the database is basically the same, except for the "like" behavior.

### this 2 service use rabbitMQ to sync data to each other.
### Ex: when admin do CRUD for the products in the "product" service, it will create message to sync to the "main" service as well.
### when client give product a "like", it will create message to sync to the "product" service as well.
