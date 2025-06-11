# Struktur Umum

1.1 Penempatan File

* Model diletakkan di `app/Models/`
* Controller di `app/Http/Controllers/`
* Form Request di `app/Http/Requests/`
* Policy di `app/Policies/`
* Event dan Listener masing-masing di `app/Events/` dan `app/Listeners/`

1.2 Prinsip Umum

* Kode harus pendek, ringkas, dan mudah dipahami.
* Setiap class hanya punya satu tanggung jawab (Single Responsibility).
* Hindari **fat controller**, **fat model**.
* Gunakan **Service Class**, **Repository Pattern**, atau **Action Class** jika logika terlalu kompleks.
