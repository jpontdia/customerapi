# Customer Profile Application - Create Customer
*Mule Project for Customer Profile Application. Feature: Create Customer*

# Table of contents
1. [Introduction](#introduction)
2. [Environment requirements](#environment-requirements)

## Introduction
In a recent Project I had the opportunity to work in the migration of a legacy Java Application from technologies like mainframe, several java and spring versions, and Weblogic app servers. These apps were migrated to the Cloud using mainly a microservices architecture. The application presented here is the partial implementation of one of the business cases: Customer Profile Service, but using MuleSoft tools. The feature implemented is Create Customer. As an entry point, We have a webservice responsible for receiving HTTP POST calls from other systems. In addition, the service validates the customer record with the business rules. If the payload complies with all regulations, it is sent to a topic in the message broker. On the consumer side, We have all the components responsible for customer creation in every company system. The following diagram shows the architecture of the application.

![Architecture diagram](/doc/CustomerProfileApplication.png)

## Environment requirements
* Anypoint Studio 7.11.0 - https://www.mulesoft.com/lp/dl/studio
  * Mule Server 4.4
* Postgresql - https://www.postgresql.org/
* RabbitMQ - https://www.rabbitmq.com/
* Stripe (Payments processor) - https://stripe.com/
