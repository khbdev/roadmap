3-HAFTA — API & Communication Protocols


---

## **Dushanba — REST API Basics**

**Nazariya:**

- REST principles (GET, POST, PUT, DELETE)
    
- Versioning, filtering, pagination
    
- Standard error response format
    
- Idempotency (POST/PUT behavior)
    

**Amaliy 1:**

- Go + Gin / Fiber bilan oddiy CRUD API yaratish
    
- Versioned endpoints (`/v1/users`, `/v2/users`)
    

**Amaliy 2 (turlicha, 1-amaliyga o‘xshamaydigan):**

- Pagination + filter query implement
    
- Standard error response format + idempotency test
    

---

## **Seshanba — REST API Validation & Middleware**

**Nazariya:**

- Validation middleware (JSON body validation, field rules)
    
- Request/Response logging
    
- Error handling best practices
    

**Amaliy 1:**

- Go middleware bilan validation implement
    
- Invalid request → error JSON return
    

**Amaliy 2 (turlicha):**

- Request logs yozish
    
- Error handling best practices qo‘shish + test
    

---

## **Chorshanba — gRPC Basics**

**Nazariya:**

- gRPC: Unary vs Streaming RPC
    
- Proto file design principles
    
- Interceptors (logging, auth)
    
- Standard error codes
    

**Amaliy 1:**

- Simple UserService proto yaratish
    
- Go gRPC server implement
    
- Unary RPC + error handling
    

**Amaliy 2 (turlicha):**

- Go gRPC client implement
    
- Unary RPC test + response validation
    
- Interceptor logging qo‘shish
    

---

## **Payshanba — gRPC Advanced**

**Nazariya:**

- Streaming RPC (server streaming, client streaming, bidirectional)
    
- Interceptors chaining
    
- Error handling & status codes
    

**Amaliy 1:**

- Go gRPC server streaming implement
    
- Logging + error interceptor qo‘shish
    

**Amaliy 2 (turlicha):**

- Client streaming / bidirectional streaming implement
    
- Live notifications yoki chat simulation
    

---

## **Juma — GraphQL Basics**

**Nazariya:**

- GraphQL schema design (Query, Mutation)
    
- Resolver concept
    
- Caching & N+1 problem
    
- Error handling
    

**Amaliy 1:**

- Go + gqlgen bilan simple GraphQL API yaratish
    
- User query implement
    

**Amaliy 2 (turlicha):**

- User mutation implement
    
- Resolver chaining va simple caching test
    

---

## **Shanba — API Gateway & Mini-Projects**

**Nazariya:**

- API Gateway concept
    
- Auth & JWT verification
    
- Rate limiting
    
- Request aggregation (multiple service → single response)
    

**Amaliy 1:**

- REST CRUD service → Users CRUD API
    
- gRPC UserService + Gateway → gRPC service + REST gateway
    

**Amaliy 2 (turlicha):**

- GraphQL Product API → gqlgen GraphQL API
    
- Gateway routing + JWT auth + rate limiter implement
    
- Mini-projectlarni alohida branch + test + README
    

---

