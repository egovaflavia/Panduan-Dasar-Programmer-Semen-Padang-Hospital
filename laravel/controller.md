# Controller

3.1 RESTful Resource

Gunakan konvensi standar Laravel:

* `index()`
* `store()`
* `show($id)`
* `update($id)`
* `destroy($id)`

3.2 Hindari:

```php
public function save(Request $request) {
    // validasi
    // simpan
    // redirect
}
```

3.3 Gunakan:

```php
public function store(UserRequest $request) {
    $data = $request->validated();
    $user = User::create($data);

    return redirect()->route('users.index');
}
```
