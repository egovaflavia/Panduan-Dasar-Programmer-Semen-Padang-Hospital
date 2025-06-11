# Dependency Injection & Service

Gunakan constructor injection:

```php
public function __construct(UserService $service)
{
    $this->service = $service;
}
```

Pisahkan logika kompleks dari controller ke `App\Services`.
