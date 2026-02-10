6-HAFTA — Testing & Best Practices


### **Dushanba — Unit & Table-driven Tests**

- **Nazariya (17:00–19:00)**
    
    - Unit test asoslari (`testing.T`)
        
    - Table-driven tests (input/output table bilan test)
        
    - Test naming conventions
        
    - Go best practices for unit testing
        
- **Amaliy (20:00–22:00)**
    
    - Oddiy function test qilish: `Add(a,b int) int`
        
    - Table-driven test: bir nechta input/output test cases
        
    - Run all tests → pass/fail check + assert & error messages bilan test report
        

---

### **Seshanba — Mocking & Integration Tests**

- **Nazariya (17:00–19:00)**
    
    - Mocking: external dependency’larni simulyatsiya qilish
        
    - Interface-based mocking
        
    - Integration tests: service + DB / API / gRPC
        
- **Amaliy (20:00–22:00)**
    
    - Go interface mocking example implement
        
    - Mock DB + unit test
        
    - Integration test: REST API + PostgreSQL / gRPC service → sample endpoint response verification
        

---

### **Chorshanba — Benchmarking & Performance**

- **Nazariya (17:00–19:00)**
    
    - Go benchmarking (`testing.B`)
        
    - Measuring performance: throughput, latency
        
    - Identifying bottlenecks
        
- **Amaliy (20:00–22:00)**
    
    - Benchmark test for CRUD API → Run & analyze throughput/latency
        
    - Compare performance with/without caching
        
    - Profiling & bottleneck identification
        

---

### **Payshanba — Logging & Error Handling**

- **Nazariya (17:00–19:00)**
    
    - Structured logging (Zap / Logrus)
        
    - Centralized error handling
        
    - Retry & backoff pattern for failed requests
        
- **Amaliy (20:00–22:00)**
    
    - Logging middleware implement → check logs output
        
    - Retry + exponential backoff for failed API calls
        
    - Simulate failed requests → verify retry logic
        

---

### **Juma — Graceful Shutdown & Health Check**

- **Nazariya (17:00–19:00)**
    
    - Graceful shutdown: signal handling (`SIGINT`, `SIGTERM`)
        
    - Health check endpoints (`/healthz`)
        
    - Config management & secrets (env variables, config file)
        
- **Amaliy (20:00–22:00)**
    
    - Go service graceful shutdown implement → send SIGINT → observe shutdown
        
    - Health check endpoint implement + verify response
        
    - Load env variables & secret keys
        

---

### **Shanba — Mini-Projects Integration**

- **Nazariya (17:00–19:00)**
    
    - Testing + reliability integration: REST + gRPC + retry/backoff + graceful shutdown
        
- **Amaliy (20:00–22:00)**
    
    - Full test coverage REST + gRPC service → Unit + integration + table-driven tests
        
    - Logs va metrics orqali behavior verify
        
    - Retry + backoff simulation → simulate failing requests → verify success
        
    - Health check + graceful shutdown → signals handle + endpoint status
        
    - Har mini-project alohida branch + README (testing strategy, retry/backoff, graceful shutdown implementation)
        

---

