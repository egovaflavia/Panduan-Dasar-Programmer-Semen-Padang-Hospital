# Komunikasi Antar Komponen

Gunakan `emit()` dan `listeners`:

```php
$this->emit('userCreated');

protected $listeners = ['userCreated' => 'reloadUsers'];
```
