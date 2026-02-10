2-HAFTA — Database Systems


---

## **Dushanba — SQL (PostgreSQL) Basics**

**Nazariya:**

- SQL CRUD: `SELECT`, `INSERT`, `UPDATE`, `DELETE`
    
- `WHERE`, `ORDER BY`, `LIMIT`
    
- `INNER JOIN`, `LEFT JOIN`
    
- Primary key va Foreign key
    

**Amaliy:**

- `users` va `orders` jadvali yaratish
    
- Foreign key bilan bog‘lash
    
- 5–10 ta record qo‘shish
    
- `JOIN` orqali user + orderlarni olish
    

**Mini-task:**

- **Go + PostgreSQL CRUD API**
    
    - GET /users
        
    - POST /users
        
    - PUT /users
        
    - DELETE /users
        

---

## **Seshanba — SQL Transactions**

**Nazariya:**

- Transaction nima?
    
- `BEGIN`, `COMMIT`, `ROLLBACK`
    
- ACID:
    
    - Atomicity
        
    - Consistency
        
    - Isolation
        
    - Durability
        

**Amaliy:**

- Go’da transaction ishlatib:
    
    - Order yaratish
        
    - Payment qo‘shish
        
    - Xatolik bo‘lsa rollback
        

**Mini-task:**

- **Transaction API**
    
    - `POST /orders`
        
    - Order + payment **bitta transaction**
        
    - Error bo‘lsa hammasi bekor bo‘lsin
        

---

## **Chorshanba — Advanced SQL Practice**



**Nazariya:**

- Index nima va nima uchun kerak
    
- `UNIQUE`, `NOT NULL`
    
- `ON DELETE CASCADE`
    
- `EXPLAIN`
    

**Amaliy:**

- Index qo‘shish (`email`, `user_id`)
    
- `users → orders` cascade delete
    
- Sekin va tez query farqini ko‘rish
    

**Mini-task:**

- **Optimized SQL API**
    
    - Index bilan ishlaydigan endpoint
        
    - `EXPLAIN` orqali tahlil
        

---

## **Payshanba — Redis Basics**

**Nazariya:**

- Redis nima?
    
- Cache-aside pattern
    
- TTL / expire
    
- Rate limiter tushunchasi
    
- Pub/Sub (faqat overview)
    

**Amaliy:**

- Redis set/get
    
- TTL bilan cache
    
- Request count limiter
    

**Mini-task:**

- **Go + Redis**
    
    - GET `/users` → Redis cache
        
    - Rate limiter: 1 user = N request / minute
        

---

## **Juma — File Storage + Redis Mapping**

**Nazariya:**

- Local storage vs Object storage
    
- File upload / download flow
    
- Redis’da mapping saqlash
    

**Amaliy:**

- Go’da file upload (`multipart/form-data`)
    
- Faylni local folderga saqlash
    
- Redis’da:
    
    ```
    file_id → file_path
    ```
    

**Mini-task:**

- **File service API**
    
    - POST `/upload`
        
    - GET `/download/{file_id}`
        

---

## **Shanba — Integration Mini-Projects**

**Maqsad:** hammasini **bitta backend skill**ga yig‘ish

### **Mini-projectlar:**

### 1️⃣ SQL + Redis Caching Service

- PostgreSQL → asosiy DB
    
- Redis → cache
    
- CRUD + cache invalidation
    

### 2️⃣ Transaction-based Order System

- Order + Payment
    
- To‘liq ACID
    
- Rollback test
    

### 3️⃣ File Upload Service

- Local storage
    
- Redis mapping
    
- Download endpoint
    

**Amaliy:**

- Har mini-project → alohida **git branch**
    
- Test qilish
    
- README yozish:
    
    - Nima qilindi
        
    - Endpointlar
        
    - Texnologiyalar
        

---

