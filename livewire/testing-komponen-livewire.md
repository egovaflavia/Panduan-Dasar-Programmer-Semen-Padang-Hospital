# Testing Komponen Livewire

Gunakan Livewire testing:

```php
public function test_user_can_submit_form()
{
    Livewire::test(CreateUser::class)
        ->set('name', 'John Doe')
        ->set('email', 'john@example.com')
        ->call('submit')
        ->assertRedirect('/users');
}
```
