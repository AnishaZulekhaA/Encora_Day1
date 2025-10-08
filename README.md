# E-commerce Microservices Project | Spring Boot & Kafka

This repository contains a sample e-commerce application implemented using Spring Boot, Maven, and Apache Kafka.  
It demonstrates a simple order management system built with a microservices architecture.

## Microservices Overview

1. **Amazon Service**  
   - Handles order creation via REST API  
   - Publishes order details to a Kafka topic

2. **Flipkart Service**  
   - Listens to the Kafka topic  
   - Displays received orders via a REST API

## Key Features

- RESTful APIs for order management
- Asynchronous communication using Apache Kafka
- Modular Maven multi-module structure
- Producer-consumer microservice design pattern
- Easily extendable to support additional platforms

## Technologies Used

- Java 21
- Spring Boot 3.3.3
- Apache Kafka
- Maven
- REST APIs

## Getting Started

To run the project locally:
1. Start your Kafka broker
2. Run `AmazonApplication` and `FlipkartApplication` separately
3. Use POST `/orders/create` to place an order
4. Use GET `/api/orders/received` to view received orders

