# Optimasi

* Gunakan `lazy` atau `debounce` untuk input yang intensif:

```html
<input wire:model.lazy="search" />
```

* Gunakan `wire:key` pada loop untuk menghindari re-render:

```php
@foreach ($users as $user)
    <div wire:key="user-{{ $user->id }}">
        {{ $user->name }}
    </div>
@endforeach
```
