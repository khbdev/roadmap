7-HAFTA — Design Patterns & Clean Code


---

## **Dushanba — Factory Pattern**

**Maqsad:** Oddiy obyekt yaratishni abstraktsiyalash va real code’da qo‘llash

### Nazariya

- Factory Pattern nima va qachon ishlatiladi
    
- Interface vs Concrete type
    
- Afzalliklar: encapsulation, decoupling
    
- Misol: logger yoki database connector yaratish
    

### Amaliy

- Oddiy `Go` struct + interface yaratish
    
- `NewProduct()` factory method bilan obyekt yaratish
    
- 2–3 turdagi obyektni bitta factory orqali yaratish
    
- Test: yangi obyekt qo‘shish → minimal code o‘zgartirish bilan
    

---

## **Seshanba — Abstract Factory Pattern**

**Maqsad:** Bir nechta bog‘langan obyektlarni bir joyda yaratish

### Nazariya

- Abstract Factory vs Factory Pattern farqi
    
- Product families tushunchasi
    
- Qachon ishlatiladi: GUI widgets, DB connectors
    
- Coupling kamaytirish
    

### Amaliy

- 2 ta product family yaratish (`Button` va `Checkbox`)
    
- `GUIFactory` interface va `WindowsFactory` / `MacFactory` concrete implementatsiyasi
    
- Test: factory o‘zgarsa → client code o‘zgarmaydi
    

---

## **Chorshanba — Builder Pattern**

**Maqsad:** Murakkab obyekt yaratishni bosqichma-bosqich abstraktsiyalash

### Nazariya

- Builder Pattern nima
    
- Director va Builder interfeysi
    
- Qachon ishlatiladi: complex object construction (reports, UI components)
    
- Real-world: Horizontal vs Vertical scaling, Stateless vs Stateful architectures
    

### Amaliy

- `Car` yoki `House` struct yaratish
    
- `Builder` interface + `CarBuilder` / `HouseBuilder`
    
- `Director` yordamida step-by-step build
    
- Test: turli config bilan 2–3 obyekt yaratish
    

---

## **Payshanba — Prototype Pattern**

**Maqsad:** Obyektni clone qilish orqali creation costni kamaytirish

### Nazariya

- Prototype Pattern nima
    
- Deep copy vs Shallow copy
    
- Qachon ishlatiladi: load balancing, performance testing
    
- Real-world: DB connection pool yoki config cloning
    

### Amaliy

- `Go` struct + `Clone()` method
    
- Object copy qil → originaldan mustaqil ishlaydi
    
- Test: 2–3 obyektni clone qilish va field o‘zgartirish
    
- Compare performance: new vs clone
    

---

## **Juma — Singleton Pattern**

**Maqsad:** Global access va single instance management

### Nazariya

- Singleton Pattern nima
    
- Thread-safe implementation (`sync.Once`)
    
- Qachon ishlatiladi: logging, configuration, caching
    
- Tech impact: Scalability, Security, Reliability & Availability, Data Management, Performance
    

### Amaliy

- `Go` da thread-safe singleton yaratish
    
- 2–3 goroutine bilan bir vaqtda singleton instance olish
    
- Test: instance har doim bitta ekanini tekshirish
    

---

## **Shanba — Pattern Integration + Mini Project**

**Maqsad:** Barcha patternlarni bir loyihada ko‘rish va integratsiya

### Nazariya

- Qaysi pattern qayerda foydali
    
- Coupling vs Cohesion tahlili
    
- Patterns combined usage (Factory + Builder + Singleton)
    

### Amaliy

- Mini Go project: `Vehicle Management System`
    
    - Factory → Vehicle yaratish
        
    - Abstract Factory → Vehicle families (Car, Bike)
        
    - Builder → Complex vehicle configuration
        
    - Prototype → Vehicle cloning
        
    - Singleton → Global registry / config
        
- Test: bir nechta vehicle create + clone + global registry check
    

---
