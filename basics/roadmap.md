# System Design – Complete Roadmap

This README provides a **structured, interview-focused roadmap** for learning **System Design**, covering **Basics → HLD → LLD → Distributed Systems → Security → Performance → Real-world case studies**.

---

## 📌 Basics

### System Design Introduction – HLD & LLD

* **HLD (High-Level Design):** Architecture, components, data flow
* **LLD (Low-Level Design):** Classes, methods, schemas, interfaces

### Functional & Non-Functional Requirements

* **Functional:** What the system does (features)
* **Non-Functional:** How well it does it (scale, latency, security)

---

## 🏗 High Level Design (HLD)

### What is High Level Design?

* Overall system architecture
* Services, databases, communication patterns

### System Architectural Styles

#### Monolithic Architecture

* Single deployable unit
* Simple, fast to start

#### Microservices Architecture

* Independently deployable services
* Scales well, operationally complex

#### Monolithic vs Microservices

| Feature    | Monolith | Microservices |
| ---------- | -------- | ------------- |
| Deployment | Single   | Independent   |
| Scaling    | Hard     | Easy          |
| Complexity | Low      | High          |

#### Event-Driven Architecture

* Producers publish events
* Consumers react asynchronously

#### Serverless Architecture

* No server management
* Pay-per-execution

#### Stateful vs Stateless Architecture

* **Stateful:** Session stored on server
* **Stateless:** Session stored externally (Redis/JWT)

#### Pub/Sub Architecture

* Decoupled communication
* Kafka, RabbitMQ, SNS/SQS

---

## 📈 Scalability

### Horizontal vs Vertical Scaling

* **Vertical:** Add more power to machine
* **Horizontal:** Add more machines

### Which Scaling Approach to Choose?

* Horizontal preferred for large-scale systems

### Primary Scalability Bottlenecks

* Database locks
* Network latency
* Disk I/O
* Synchronous dependencies

---

## 🗄 Databases in System Design

### Choosing SQL vs NoSQL

| SQL        | NoSQL                 |
| ---------- | --------------------- |
| ACID       | Eventually consistent |
| Joins      | Denormalized          |
| Structured | Flexible schema       |

### File & Database Storage Systems

* Block Storage
* Object Storage
* File Storage

### Database Replication

* Master-Slave
* Multi-master

### Database Sharding

* Horizontal partitioning
* Shard key selection critical

### Storage Types

* **Block:** Databases
* **Object:** Images, videos
* **File:** Shared filesystems

### Normalization (DBMS)

* Reduce redundancy

### Denormalization

* Improve read performance

### SQL Query Optimization

* Indexing
* Query plans
* Avoid SELECT *

### Redis Introduction

* In-memory data store
* Cache, rate limiting, session store

---

## ⚖ Consistency, Availability & Reliability

### Availability

* System uptime

### High Availability Techniques

* Load balancers
* Replication
* Failover

### Consistency

* Data correctness across nodes

### Consistency Patterns

* Strong
* Eventual
* Read-your-writes

### CAP Theorem

* Consistency
* Availability
* Partition Tolerance

### Reliability & Fault Tolerance

* Retry
* Circuit breaker
* Graceful degradation

### Maintainability

* Modular code
* Observability
* Documentation

---

## ⚙ Load Balancing

### Load Balancer

* Distributes traffic

### Load Balancing Algorithms

* Round Robin
* Least Connections
* IP Hash

### Consistent Hashing

* Reduces rebalancing during scale

---

## 🚀 Latency, Throughput & Caching

### Latency vs Throughput

* Latency: Response time
* Throughput: Requests/sec

### Caching

* Client-side
* CDN
* Redis
* Cache-aside pattern

---

## 🔌 API Gateway, Queues & Rate Limiting

### API Gateway

* Authentication
* Routing
* Rate limiting

### Message Queues

* Kafka
* RabbitMQ
* SQS

### Rate Limiting

* Protects APIs

### Rate Limiting Algorithms

* Token Bucket
* Leaky Bucket
* Sliding Window

---

## 🌐 Protocols, CDN & WebSockets

### Communication Protocols

* HTTP/HTTPS
* gRPC
* WebSocket

### DNS & DNS Caching

* Domain resolution
* TTL-based caching

### CDN

* Serve static content closer to users

### Proxies

* Forward Proxy
* Reverse Proxy

### WebSockets

* Bi-directional communication

---

## 🧪 Testing & CI/CD

### Unit Testing

* Test individual components

### Integration Testing

* Test service interactions

### CI/CD Pipeline

* Build → Test → Deploy

---

## 🔐 Security Measures

### Authentication & Authorization

* JWT
* OAuth2

### SSL / TLS

* Encrypted communication

### SSDLC

* Security at every SDLC phase

### Data Backup & Disaster Recovery

* Snapshots
* Multi-region backup

---

## 🌍 Distributed System Design

### Consensus Algorithms

* Raft
* Paxos

### Distributed Tracing

* OpenTelemetry
* Zipkin

### Secure Communication

* mTLS

---

## 💰 Cost & Performance Optimization

### Software Cost Estimation

* Infra
* Storage
* Compute

### Performance Optimization

* Async processing
* Caching
* Batching

---

## 🧩 Low Level Design (LLD)

### Core Concepts

#### Object-Oriented Programming

* Encapsulation
* Inheritance
* Polymorphism
* Abstraction

#### Modularity & Interfaces

* Loose coupling

### What is LLD?

* Class diagrams
* APIs
* DB schemas

---

## 📐 Design Principles

* SOLID
* DRY
* KISS
* YAGNI

---

## 📊 UML

### Unified Modeling Language

* Class Diagram
* Sequence Diagram
* Use Case Diagram

---

## 🧠 Design Patterns

### Creational

* Singleton
* Factory Method
* Abstract Factory
* Builder
* Prototype

### Structural

* Adapter
* Decorator
* Composite
* Proxy
* Facade

### Behavioral

* Observer
* Strategy
* Command
* State
* Template Method

---

## 🧪 System Design Interview Questions

* URL Shortening Service
* Dropbox
* Twitter
* Netflix
* Uber
* BookMyShow
* Facebook Messenger
* WhatsApp
* Instagram
* Airbnb
* Airline Management System

---

## 📚 How to Use This Repository

* Learn concepts in order
* Practice real-world designs
* Focus on trade-offs
* Think scalability & failure first

---

🚀 **Master this roadmap and you’ll be ready for Senior / Staff-level System Design interviews.**
