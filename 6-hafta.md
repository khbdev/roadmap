

# 🧪 6-HAFTA — Testing & Best Practices

## 📅 **Chorshanba → Yakshanba**

---

## 🟡 **Chorshanba — Unit & Table-driven Tests**

### **Nazariya (17:00–19:00)**

* `testing` paketi:

  * `TestXxx(t *testing.T)`
  * `t.Run`, `t.Errorf`
* Table-driven tests:

  * `[]struct{ name, input, expected }`
* Test naming:

  * `TestAdd_PositiveNumbers`
* Unit test best practices:

  * 1 test = 1 behavior
  * external dependency yo‘q

### **Amaliy (20:00–22:00)**

* `Add(a, b int) int`
* Oddiy unit test
* Table-driven test:

  * positive
  * negative
  * zero
* `go test ./...`
* Fail bo‘lsa → error message o‘qish

🎯 **Natija:**

> Unit test yozish refleksga aylanadi

---

## 🟡 **Payshanba — Mocking & Integration Tests**

### **Nazariya (17:00–19:00)**

* Mocking nima uchun kerak
* Interface-based design
* Unit vs Integration test farqi
* Qachon DB ko‘tariladi, qachon yo‘q

### **Amaliy (20:00–22:00)**

* Interface:

  ```go
  type UserRepo interface {
      GetByID(id int) (*User, error)
  }
  ```
* Mock implementatsiya
* Unit test (DBsiz)
* Integration test:

  * REST API
  * PostgreSQL (docker yoki test DB)
* Response verify

🎯 **Natija:**

> “Test DB yoqmasdan ham test yozaman” daraja

---

## 🟡 **Juma — Benchmarking & Performance**

### **Nazariya (17:00–19:00)**

* `BenchmarkXxx(b *testing.B)`
* `b.ResetTimer()`
* Throughput vs latency
* Qachon optimize qilish kerak

### **Amaliy (20:00–22:00)**

* CRUD API benchmark
* `go test -bench=.`
* Cache yo‘q holat vs cache bilan
* Natijani solishtir
* Bottleneck top

🎯 **Natija:**

> “Bu joy sekin”ni **raqam bilan** ayta olasan

---

## 🟡 **Shanba — Logging & Error Handling**

### **Nazariya (17:00–19:00)**

* Structured logging:

  * zap / logrus
* Error wrapping:

  * `fmt.Errorf("x: %w", err)`
* Retry & backoff pattern
* Log ≠ println

### **Amaliy (20:00–22:00)**

* Logging middleware
* Request ID bilan log
* Retry + exponential backoff
* Xato so‘rov simulyatsiya
* Log outputni tahlil qil

🎯 **Natija:**

> Prod’da logdan muammo topa olasan

---

## 🟡 **Yakshanba — Graceful Shutdown & Health Check**

### **Nazariya (17:00–19:00)**

* `SIGINT`, `SIGTERM`
* Graceful shutdown nima uchun muhim
* `/healthz`, `/readyz`
* Config & secrets:

  * `.env`
  * environment separation

### **Amaliy (20:00–22:00)**

* Graceful shutdown:

  * `context.WithCancel`
  * `signal.Notify`
* Serverni to‘xtat → active request tugasin
* Health check endpoint
* Env variable load

🎯 **Natija:**

> **Production-grade Go service**

---
