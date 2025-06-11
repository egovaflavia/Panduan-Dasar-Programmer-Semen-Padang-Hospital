# Lingkungan dan .env

Setiap environment memiliki file konfigurasi yang sesuai. Gunakan file `.env` dengan bijak dan **jangan pernah commit file `.env` ke repository**.

* `.env` – Digunakan untuk development lokal.
* `.env.testing` – Digunakan oleh pipeline testing.
* `.env.production` – Digunakan di server produksi.
* Setiap environment (dev/testing/production) menggunakan file `.env` yang berbeda.
* Jangan pernah commit `.env` ke Git.
* Simpan nilai sensitif seperti API\_KEY, DB\_PASSWORD, APP\_SECRET di `.env`.
* Pastikan konfigurasi `config/*.php` mengambil nilai dari `env()` dan bukan hardcode.
