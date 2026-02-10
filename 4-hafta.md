4-HAFTA — Message Brokers & Async Systems


### **Dushanba — RabbitMQ Basics**

- **Nazariya 
    
    - RabbitMQ nima va nima uchun kerak
        
    - Exchanges: direct, topic, fanout
        
    - Routing keys tushunchasi
        
    - Producer / Consumer modeli
        
- **Amaliy **
    
    - Go’da RabbitMQ connection ochish
        
    - Oddiy direct exchange bilan message yuborish va olish
        
    - Routing key bilan filter qilish
        
    - `"Hello World"` message producer + consumer test
        

---

### **Seshanba — RabbitMQ Advanced**

- **Nazariya (17:00–19:00)**
    
    - Ack / Nack + retry pattern
        
    - Dead letter queues (DLQ)
        
    - Idempotency pattern: message qayta ishlanmasligi
        
- **Amaliy (20:00–22:00)**
    
    - Go’da message process + ack / nack implement
        
    - Failed messages DLQ’ga yuborish
        
    - Simple retry logic implement
        
    - Worker API: 1 failed message → retry → DLQ test
        

---

### **Chorshanba — Kafka Basics**

- **Nazariya 
    
    - Kafka topic / partition / consumer group
        
    - Offset management: commit / auto-commit
        
    - Event ordering principles
        
    - Delivery semantics: at-least-once, exactly-once
        
- **Amaliy **
    
    - Go + Kafka: topic yaratish
        
    - Producer bilan message yuborish
        
    - Consumer group bilan read qilish
        
    - 10–20 messages producer/consumer test
        

---

### **Payshanba — Kafka Advanced**

- **Nazariya (17:00–19:00)**
    
    - Event ordering + partition key
        
    - Consumer group rebalancing
        
    - Idempotency in Kafka
        
- **Amaliy (20:00–22:00)**
    
    - Go consumer offset management test
        
    - Multiple partitions → message ordering verify
        
    - Simple idempotency check
---

### **Juma — Background Worker Pool**

- **Nazariya**
    
    - Worker pool pattern: fan-out / fan-in
        
    - Retry mechanism + backoff strategy
        
    - Non-blocking system principles
        
- **Amaliy **
    
    - Go’da 3–5 worker goroutine
        
    - Task queue (channel / message broker)
        
    - Retry & backoff implement
        
    - Background email notification queue (RabbitMQ) test
        

---

### **Shanba — Mini-Projects Integration**

- **Nazariya (17:00–19:00)**
    
    - Mini-project integration: RabbitMQ + Kafka + Worker pool
        
- **Amaliy (20:00–22:00)**
    
    - Email notification queue → RabbitMQ + worker pool, Retry + DLQ implement
        
    - Event-driven user activity log → Kafka topic → Go consumer → store / print
        
    - Background worker pool with retries → fan-out/fan-in workers + retry failed tasks
        
    - Har mini-project alohida branch + test + logs verify
        
    - README yozish: “nima qilindi, qanday ishlaydi, message flow”
        

---

