# Model & Eloquent

Eager Loading

Selalu gunakan `with()` jika akses relasi:

```php
User::with('profile')->get();
```

Accessor & Mutator

Gunakan untuk manipulasi data:

```php
public function getFullNameAttribute()
{
    return "{$this->first_name} {$this->last_name}";
}
```
