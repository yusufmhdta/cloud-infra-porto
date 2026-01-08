# Web Server Deployment (Nginx)

## Objective
Menjalankan web application sederhana menggunakan Nginx pada Google Compute Engine VM sebagai bagian dari Cloud Infrastructure Operations.

---

## Environment
- Cloud Provider: Google Cloud Platform (GCP)
- Service: Compute Engine
- OS: Ubuntu 20.04 LTS
- Web Server: Nginx

---

## Steps

### 1. Create Compute Engine VM
- Machine type: e2-micro
- Region & Zone: default
- Allow HTTP traffic: enabled

---

### 2. Access VM via SSH
Gunakan SSH dari Google Cloud Console.

---

### 3. Install Nginx
```bash
sudo apt update
sudo apt install nginx -y
