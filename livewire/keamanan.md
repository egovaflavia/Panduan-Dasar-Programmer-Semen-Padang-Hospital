# Keamanan

* Jangan expose data sensitif sebagai properti publik.
* Validasi wajib dilakukan sebelum proses penyimpanan.
* Gunakan Laravel Authorization (Policy/Gate) bila diperlukan:

```php
$this->authorize('create', User::class);
```
