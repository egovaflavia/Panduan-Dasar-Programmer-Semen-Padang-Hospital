# Validasi

Gunakan Form Request:

```bash
php artisan make:request StoreUserRequest
```

```php
public function rules()
{
    return [
        'name' => 'required|string|max:255',
        'email' => 'required|email|unique:users,email',
    ];
}
```
