# Aturan Kode Komponen Livewire

3.1 Binding Data

Gunakan properti publik untuk binding:

```php
public $name, $email;
```

Pada Blade:

```html
<input wire:model="name" type="text" />
```

**3.2 Validasi Data**

Lakukan validasi dalam `rules()` atau metode:

```php
protected $rules = [
    'name' => 'required|string',
    'email' => 'required|email|unique:users',
];

public function submit()
{
    $this->validate();
    User::create($this->only(['name', 'email']));
}
```

**3.3 Lifecycle Hooks**

Gunakan hook seperti:

* `mount()`: untuk inisialisasi data
* `updated()`: menangani perubahan properti
* `render()`: mengembalikan view

Contoh:

```php
public function mount()
{
    $this->name = 'Guest';
}
```
