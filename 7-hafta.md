
8-HAFTA — Architecture & System Design
---
### **Dushanba — Architecture Patterns Basics**

- **Nazariya (17:00–19:00)**
    
    - Monolith vs Modular Monolith
        
    - Microservices overview
        
    - Event-driven architecture basics
        
    - Qaysi holatda qaysi pattern ishlatiladi
        
- **Amaliy (20:00–22:00)**
    
    - Oddiy monolith API yaratish (Users + Orders CRUD)
        
    - Modular Monolith: service’larni package / folder bilan modulga ajratish → CRUD + modular structure test
        

---

### **Seshanba — Microservices Design**

- **Nazariya (17:00–19:00)**
    
    - Microservices principles: single responsibility, independent deploy
        
    - Service communication: REST / gRPC / message broker
        
    - Service isolation + failure handling
        
- **Amaliy (20:00–22:00)**
    
    - Monolith API’ni 2–3 microservice’ga bo‘lish (UserService, OrderService)
        
    - Microservice inter-service communication test → CRUD endpoints + internal communication verification
        

---

### **Chorshanba — Event-driven Architecture**

- **Nazariya (17:00–19:00)**
    
    - Event-driven concepts: publisher / subscriber
        
    - Saga vs Choreography pattern
        
    - Event queues (RabbitMQ/Kafka)
        
    - Idempotency, retries
        
- **Amaliy (20:00–22:00)**
    
    - User registration → event published → OrderService listens
        
    - Simple saga: order creation → payment → notification
        
    - Event-driven order processing mini-project start
        

---

### **Payshanba — System Design Principles**

- **Nazariya (17:00–19:00)**
    
    - Scalability: vertical vs horizontal
        
    - Availability, Consistency
        
    - CAP theorem overview
        
    - Caching strategies: cache-aside, read-through, write-through
        
- **Amaliy (20:00–22:00)**
    
    - Go API + Redis cache layer implement
        
    - Simple fallback on cache miss / DB read
        
    - Cache layer + fallback test
        

---

### **Juma — Failure Handling & Advanced Design**

- **Nazariya (17:00–19:00)**
    
    - Circuit breaker pattern
        
    - Retry + backoff
        
    - Service isolation (fail fast, degrade gracefully)
        
    - Logging & monitoring importance
        
- **Amaliy (20:00–22:00)**
    
    - Go service: retry failed requests + fallback implement
        
    - Circuit breaker implement (simple library / custom)
        
    - Background task retry + fallback simulation
        

---

### **Shanba — Mini-Projects Integration**

- **Nazariya (17:00–19:00)**
    
    - Architecture + Microservices + Event-driven integration
        
- **Amaliy (20:00–22:00)**
    
    - Monolith → Microservices refactor
        
    - Event-driven order processing system (User registration → Order creation → Notification via RabbitMQ/Kafka)
        
    - Cache layer + fallback: Redis caching + fallback DB read
        
    - Har mini-project alohida branch + Logs, retries, fallback, monitoring test
        
    - README: nima qilindi, service flow, design decisions
        

---


