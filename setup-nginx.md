# Web Server Deployment (Nginx)

## Objective
Menjalankan web application sederhana menggunakan Nginx pada Google Compute Engine VM sebagai bagian dari Cloud Infrastructure Operations.

---

## Environment
- Cloud Provider: Google Cloud Platform (GCP)
- Service: Compute Engine
- OS: Ubuntu 24.04 LTS
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
```
---

### 4. Start & Enable Nginx
```bash
sudo systemctl start nginx
sudo systemctl enable nginx
```
---

### 5. Verify Web Server

Akses melalui browser (Windows)

```bash
http://localhost:8080
```

Jika muncul halaman default Nginx berarti deployment berhasil.

---

### Result

<img width="797" height="301" alt="{F8860C85-F8B8-4CF2-88DE-B2D0DF7D10E8}" src="https://github.com/user-attachments/assets/59e6b5c4-4cca-4111-b4e0-80127daf87f6" />

