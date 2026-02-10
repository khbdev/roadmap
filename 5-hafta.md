
# 🧱 5-HAFTA — DevOps, Cloud & Final System

## 📅 **Chorshanba → Yakshanba**

---

## 🟡 **Chorshanba — Docker Basics & Multi-stage Builds**

### **Nazariya (17:00–19:00)**

* Docker nima:

  * image vs container
  * Dockerfile
* Container vs VM (intervyu savol!)
* Multi-stage build:

  * build image
  * runtime image
  * nega prod’da muhim

### **Amaliy (20:00–22:00)**

* Oddiy Go REST API yoz:

  * `/ping` → `"ok"`
* Dockerfile:

  * `docker build`
  * `docker run`
* Multi-stage Dockerfile:

  * `golang:alpine` → build
  * `scratch/alpine` → run
* Endpoint test:

  * `curl localhost:8080/ping`

🎯 **Natija:**

> Go service → **minimal production Docker image**

---

## 🟡 **Payshanba — docker-compose & Local Dev Environment**

### **Nazariya (17:00–19:00)**

* docker-compose nima uchun kerak
* Service networking
* Volumes (DB data yo‘qolmasligi uchun)
* Logs & restart policy

### **Amaliy (20:00–22:00)**

* `docker-compose.yml`:

  * Go API
  * PostgreSQL
  * Redis
* `.env` bilan config
* `docker-compose up -d`
* Tekshir:

  * API ishlayaptimi
  * DB ulanadimi
  * Redis ping

🎯 **Natija:**

> **Local production-like environment**

---

## 🟡 **Juma — CI/CD Basics (GitHub Actions)**

### **Nazariya (17:00–19:00)**

* CI/CD pipeline flow:

  * push → build → test → image
* GitHub Actions:

  * jobs
  * steps
  * runners
* Lint & test nima uchun muhim

### **Amaliy (20:00–22:00)**

* `.github/workflows/ci.yml`
* Pipeline:

  * `go test ./...`
  * `go vet`
  * Docker image build
* Push qil → pipeline ishlaganini ko‘r

🎯 **Natija:**

> **Push = avtomatik tekshiruv + build**

---

## 🟡 **Shanba — Cloud & Infrastructure (VPS)**

### **Nazariya (17:00–19:00)**

* VPS nima
* Linux server setup
* Nginx reverse proxy
* Environment variables & secrets
* SSL (Let’s Encrypt)

### **Amaliy (20:00–22:00)**

* VPS (Ubuntu):

  * Docker install
  * docker-compose install
* Go service deploy
* Nginx:

  * reverse proxy
* HTTPS:

  * Certbot
* Domain orqali API ochilishini tekshir

🎯 **Natija:**

> **Real internetga chiqgan backend service**

---

## 🟡 **Yakshanba — Monitoring, Logging & Final Polish**

### **Nazariya (17:00–19:00)**

* Monitoring nima:

  * metrics
  * logs
* Health checks
* Prometheus / Grafana overview
* Observability mindset

### **Amaliy (20:00–22:00)**

* `/health` endpoint
* Prometheus metrics (`/metrics`)
* Grafana dashboard (basic)
* Logs:

  * stdout
  * docker logs
* Service o‘chsa → qayta ishga tushishini test qil

🎯 **Natija:**

> **Production-ready backend**

---

