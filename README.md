# Scuti/AdminMetronic
This is admin template base on Admin Metronic theme (https://keenthemes.com/metronic/).

# How to install

### Step 1: Install via composer

```php
composer require scuti/admin-metronic
```

### Step 2: Publish metronic admin theme

```php
php artisan vendor:publish --tag=admin-metronic --force
```

### Step 3: Make a route to display show admin and enjoy!

```
Route::get('/admin', function () {
    return view('admin.index');
});

Route::get('/login', function () {
    return view('auth.login');
});

Route::get('password/reset', function () {
    return view('auth.passwords.email');
})->name('password.reset');

Route::get('/profile', function () {
    return view('auth.profile');
})->name('profile.edit');

Route::get('/change-password', function () {
    return view('auth.passwords.change');
})->name('auth.password.edit');
```
# admin-metronic
