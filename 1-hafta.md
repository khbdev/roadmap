1-HAFTA — Concurrency

---

## **Dushanba — Concurrency Fundamentals (Asoslar)**

**Maqsad:** Concurrency nima ekanini tushunish, parallel vs concurrency farqi

### Nazariya

- Concurrency vs Parallelism (muhim!)
    
- OS Thread vs Goroutine
    
- Goroutine lifecycle
    
- `runtime.GOMAXPROCS`
    
- `runtime.NumCPU()`
    

### Amaliy

- Oddiy goroutine yaratish
    
- `main` tugashi bilan goroutine o‘lishini ko‘rish
    
- `time.Sleep` bilan vaqt berish
    
- Bir vaqtning o‘zida 3–5 goroutine ishini kuzatish
    

📌 **Nega bu kun muhim?**  
Agar shu tushunilmasa, channel va select **umuman o‘tirmaydi**.

---

## **Seshanba — Goroutine + WaitGroup**

**Maqsad:** Goroutine’larni boshqarish va tugashini kutish

### Nazariya

- `go func() {}()`
    
- Goroutine’ning yengilligi
    
- `sync.WaitGroup` (`Add`, `Done`, `Wait`)
    
- Goroutine leak tushunchasi
    

### Amaliy

- Loop ichida 10–20 goroutine
    
- Har biri `time.Sleep` bilan ishlaydi
    
- `WaitGroup`siz va `WaitGroup` bilan farqni ko‘rish
    
- Output tartibsiz chiqishini tahlil qilish
    

---

## **Chorshanba — Channel Asoslari**

**Maqsad:** Goroutine’lar o‘rtasida to‘g‘ri aloqa o‘rnatish

### Nazariya

- Channel nima va nega kerak
    
- Unbuffered channel (blocking)
    
- Buffered channel (queue kabi)
    
- Send / Receive
    
- `close(ch)` va `range ch`
    

### Amaliy

- 1 producer → 1 consumer
    
- 5 producer → 1 consumer
    
- Buffered vs unbuffered test
    
- Deadlock holatini ataylab chiqarish
    

📌 **Bu kunda DEADLOCK ni ko‘rmasang — yomon o‘rganilgan bo‘ladi**

---

## **Payshanba — Select, Timeout, Cancel**

**Maqsad:** Real-world control (timeout, cancel)

### Nazariya

- `select` qanday ishlaydi
    
- Multiple channel bilan ishlash
    
- `time.After`
    
- Cancel pattern:
    
    - channel orqali
        
    - `context.Context` (basic level)
        

### Amaliy

- Goroutine 2 soniyadan oshsa → cancel
    
- 2 ta channel’dan birini tanlab o‘qish
    
- `select { default: }` bilan non-blocking read
    

📌 **Bu kun seni junior → middlega olib chiqadi**

---

## **Juma — Worker Pool (Fan-in / Fan-out)**

**Maqsad:** Production’da ishlatiladigan pattern

### Nazariya

- Fan-out (tasks → workers)
    
- Fan-in (results → collector)
    
- Worker pool arxitekturasi
    
- Backpressure tushunchasi
    

### Amaliy

- 1 producer
    
- 3 worker goroutine
    
- Task: `n*n`
    
- Barcha natijani bitta channel’da yig‘ish
    
- Worker graceful shutdown
    

📌 **Bu intervyuda ENG KO‘P so‘raladigan pattern**

---

## **Shanba — Mutex, Race condition & Testing**

**Maqsad:** Xavfsiz parallel kod yozish + test

### Nazariya

- Race condition nima
    
- `sync.Mutex`
    
- `sync.RWMutex`
    
- `go test`
    
- Table-driven tests
    

### Amaliy

- Shared counter → race
    
- Mutex bilan tuzatish
    
- `go test -race` ishlatish
    
- `Add(a, b int)` uchun unit test
    

---


