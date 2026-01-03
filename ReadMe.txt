Project Kelompok 3-Database Service Menggunakan Docker

A. Anggota Kelompok
- Fitri Rahmadiani (062430701469)
- Muhammad Abdurrahman (062430701476)
- Muhammad Rossi (062430701479)

B. Deskripsi
Project ini bertujuan untuk membuat service database MySQL menggunakan Docker dengan fitur persistent storage sehingga data tetap tersimpan meskipun container dihentikan atau direstart. Untuk mempermudah pengelolaan database digunakan phpMyAdmin.


C. Teknologi
- Docker
- MySQL
- phpMyAdmin
- Docker Volume

D. Cara Menjalankan
1. Install Docker Desktop
2. Masuk ke folder project
2. Jalankan:
   docker compose up -d
3. Akses database:
   - phpMyAdmin: http://localhost:8080
   - Username: admin
   - Password: admin123
4. Pengujian persistent storage
   - buat table dan data di phpMyAdmin
   - stop container: docker compose down
5. Jalankan ulang:
   docker compose up -d
6. Data tetap ada >> BERHASIL

E. Struktur File
mysql-docker/
│
├── docker-compose.yml
├── Dockerfile
├── README.md
└── video-demo
    
