

# 🔥 6-HAFTA — Design Patterns (SENING FORMATDA)

---

# 🟢 DUSHANBA — Factory Pattern

### 🎯 Maqsad:

Object creation’ni abstrakt qilish

---

### P1 – Nazariya

* Factory nima?
* Qachon kerak?
* new dan farqi nima?

### P2 – Amaliy

* Product interface
* 2 ta concrete type (FileLogger, DBLogger)

---

### P3 – Nazariya

* Encapsulation
* Decoupling
* Open/Closed Principle

### P4 – Amaliy

* `NewLogger(type string)` factory method yoz
* Switch orqali object qaytar

---

### 30 min dam

---

### P5 – Nazariya

* Factory vs simple constructor farqi
* Qachon overengineering?

### P6 – Amaliy

* Yangi logger turi qo‘sh
* Client code o‘zgarmasin

---

### P7 – Nazariya

* Real backend misol (DB connector, payment provider)

### P8 – Amaliy

* Kichik test yoz
* README ga tradeoff yoz

---

# 🟢 SESHANBA — Abstract Factory

---

### P1 – Nazariya

* Factory vs Abstract Factory farqi

### P2 – Amaliy

* Button + Checkbox interface yoz

---

### P3 – Nazariya

* Product families tushunchasi

### P4 – Amaliy

* WindowsFactory implement qil

---

### 30 min dam

---

### P5 – Nazariya

* Coupling kamayishi

### P6 – Amaliy

* MacFactory qo‘sh

---

### P7 – Nazariya

* Client code factory almashtirganda nima bo‘ladi?

### P8 – Amaliy

* Factory ni o‘zgartirib test qil
* Client o‘zgarmasin

---

# 🟢 CHORSHANBA — Builder

---

### P1 – Nazariya

* Builder nima?
* Qachon Factory yetmaydi?

### P2 – Amaliy

* Car struct yoz

---

### P3 – Nazariya

* Builder interface

### P4 – Amaliy

* CarBuilder yoz

---

### 30 min dam

---

### P5 – Nazariya

* Director roli

### P6 – Amaliy

* Director qo‘sh

---

### P7 – Nazariya

* Builder vs telescoping constructor

### P8 – Amaliy

* 2 xil config bilan car yarat

---

# 🟢 PAYSHANBA — Prototype

---

### P1 – Nazariya

* Prototype nima?
* Deep vs Shallow copy

### P2 – Amaliy

* Clone() method yoz

---

### P3 – Nazariya

* Performance foydasi

### P4 – Amaliy

* Clone qilingan object field o‘zgartir

---

### 30 min dam

---

### P5 – Nazariya

* Real use case (config cloning, pooling)

### P6 – Amaliy

* 3 ta clone yarat

---

### P7 – Nazariya

* Qachon ishlatmaslik kerak?

### P8 – Amaliy

* Simple benchmark (new vs clone)

---

# 🟢 JUMA — Singleton

---

### P1 – Nazariya

* Singleton nima?
* Qachon zararli?

### P2 – Amaliy

* Basic singleton yoz

---

### P3 – Nazariya

* Thread-safety muammosi

### P4 – Amaliy

* sync.Once bilan yoz

---

### 30 min dam

---

### P5 – Nazariya

* Global state xavfi

### P6 – Amaliy

* 3 goroutine test

---

### P7 – Nazariya

* DI vs Singleton

### P8 – Amaliy

* Test: instance har doim bitta

---

# 🟢 SHANBA — Integration Day

---

### P1 – Nazariya

* Qaysi pattern qayerda ishladi?

### P2 – Amaliy

* Vehicle interface yoz

---

### P3 – Nazariya

* Patternlarni kombinatsiya qilish

### P4 – Amaliy

* Factory + Abstract Factory qo‘sh

---

### 30 min dam

---

### P5 – Nazariya

* Cohesion vs Coupling

### P6 – Amaliy

* Builder + Prototype qo‘sh

---

### P7 – Nazariya

* Global config qayerda?

### P8 – Amaliy

* Singleton registry qo‘sh
* README yoz

---

