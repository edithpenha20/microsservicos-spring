# Arquitetura baseada em microsserviços usando spring cloud

Neste projeto foi criado um microsserviço utilizando as tecnologias ElasticSearch e Redis que se comunicaram a partir de um config server. 
Também utilizou-se como interface gráfica para melhor monitoramento dos serviços o Eureka Server.

## O que foi utilizado...

- Java 11;
- Maven;
- Spring Web;
- Actuator.
- No product-catalog utilizou-se ElasticSearch;
- No shopping-cart utilizou-se Redis;
- No server (config-server) utilizou-se Spring Cloud Config Server;
- No discovery utilizou-se Spring Cloud Eureka Server;
- E no gateway utilizou-se Spring Cloud Gateway.


## Comandos utilizados no ElasticSearch:

product-catalog: 
```
http http://localhost:8080/actuator/health
http POST http://localhost:8080/product id=1 name=mouse amount=1
http GET http://localhost:8080/product/1
http DELETE http://localhost:8080/product/1
```
