# Portal Berita Sekolah

Portal Berita Sekolah adalah platform berbasis web yang menyajikan berita sekolah dalam bentuk video yang di-embed dari YouTube. Portal ini dilengkapi dengan chatbot Telegram yang memungkinkan admin untuk melakukan CRUD berita serta mendapatkan analitik tanpa perlu login ke dashboard. Selain itu, sistem ini juga menggunakan database vektor untuk merekomendasikan berita terkait.

## Fitur Utama
- **Embed Video YouTube**: Berita ditampilkan dalam bentuk video yang diambil dari YouTube.
- **Chatbot Telegram**: Memungkinkan admin untuk menambahkan, mengedit, menghapus berita, serta melihat analitik langsung dari Telegram.
- **Analitik Berita**: Menyediakan statistik dan wawasan mengenai performa berita.
- **Rekomendasi Berita Terkait**: Menggunakan PostgreSQL dengan ekstensi `pgvector` untuk memberikan rekomendasi berita serupa.

## Teknologi yang Digunakan
- **Backend**: Laravel
- **Database**: PostgreSQL (pgvector untuk rekomendasi berita)
- **Bot**: Telegram Bot API

## Cara Deploy
1. Clone repository ini.
2. Install dependensi dengan menjalankan:
   ```sh
   composer install
   ```
3. Buat file `.env` dan sesuaikan konfigurasi database serta API key Telegram.
4. Jalankan migrasi database:
   ```sh
   php artisan migrate
   ```
5. Jalankan server Laravel:
   ```sh
   php artisan serve
   ```

## Konfigurasi
Untuk menjalankan chatbot Telegram, Anda perlu menambahkan API key Telegram pada file `.env`:
```
TELEGRAM_BOT_TOKEN=your_telegram_bot_api_key
```

## Dokumentasi Lengkap
Dokumentasi lengkap mengenai penggunaan website dan chatbot tersedia di:
[Portal Berita Sekolah - Notion](https://nervous-archduke-1bc.notion.site/Portal-Berita-Sekolah-180abda40d3b8015841bc83bfaa6d4b2?pvs=74)

## Lisensi
Proyek ini dilisensikan di bawah **Creative Commons Attribution (CC BY)**.

---

