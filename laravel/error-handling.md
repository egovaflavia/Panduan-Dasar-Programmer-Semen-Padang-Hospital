# Error Handling

* Gunakan try-catch untuk operasi berisiko.
* Gunakan custom exception untuk kasus spesifik.
* Laporkan error kritis via log:

```php
Log::error('Error creating user', ['error' => $e->getMessage()]);
```
