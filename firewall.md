# Security Configuration

## Objective
Menerapkan keamanan dasar pada infrastruktur cloud dengan prinsip least privilege.

---

## Firewall Configuration

### Firewall Rule
- Direction: Ingress
- Action: Allow
- Protocol & Port: TCP:80
- Source IP: 0.0.0.0/0
- Target: VM with network tag (http-server)

---

## IAM Configuration

### IAM Principle
Menggunakan prinsip **Least Privilege**, hanya role yang dibutuhkan saja.

### Role Used
- Compute Engine Viewer / Admin (untuk kebutuhan deploy)
- Tidak menggunakan owner secara berlebihan

---

## Security Awareness
- Port yang dibuka hanya HTTP
- Akses admin dibatasi
- Tidak menyimpan credential di VM

---

## Conclusion
Konfigurasi keamanan cukup untuk lingkungan demonstrasi portofolio magang.
