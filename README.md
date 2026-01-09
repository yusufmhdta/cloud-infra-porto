# Monitoring & Operational Evidence

## Objective
Melakukan pemantauan kondisi operasional sistem untuk memastikan web server berjalan stabil dan resource digunakan secara wajar sebagai bagian dari Cloud Infrastructure Operations.

---

## Monitoring Tool
- Tool: htop
- Type: System-level monitoring (local)
- Environment: Ubuntu Linux (VirtualBox VM)

htop dipilih karena merupakan tools bawaan Linux yang ringan, real-time, dan umum digunakan oleh system administrator untuk monitoring operasional harian.

---

## Metrics Monitored
Monitoring difokuskan pada metrik dasar yang relevan untuk operasional server, yaitu:

1. CPU Usage  
   Untuk memastikan beban server berada dalam batas normal dan tidak mengalami overload.

2. Memory Usage  
   Untuk memantau penggunaan RAM oleh sistem dan proses web server.

3. Process Status  
   Untuk memastikan proses `nginx` berjalan dengan normal.

---

## Monitoring Procedure

### 1. Menjalankan htop
Monitoring dilakukan dengan menjalankan perintah berikut pada VM:

```bash
htop
```

### 2. Observasi Resource
Pada tampilan htop, dilakukan observasi terhadap:

- Persentase CPU usage (per core)
- Total memory usage
- Load average sistem

---

### 3. Validasi Web Server Process
Proses nginx diverifikasi pada daftar process untuk memastikan:

- Status: running
- Tidak terjadi crash atau zombie process
---
Monitoring Result

Hasil monitoring menunjukkan bahwa:

- CPU usage berada pada level normal
- Memory usage stabil
- Proses Nginx berjalan dengan baik tanpa error

---

<img width="810" height="590" alt="{75578EFC-A80E-41A7-9E98-92A3E5D18849}" src="https://github.com/user-attachments/assets/96a05224-d6b9-4ea0-83f5-ff9bbffbd41f" />

