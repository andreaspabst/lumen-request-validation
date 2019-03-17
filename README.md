# Lumen Request Validation
Adds the well known Laravel ability to separate validations from the controller.

## Installation
First use composer to install the package..
 
`composer require andreaspabst/lumen-request-validation`

Next register the packages service provider in your *bootstrap/app.php* 

`$app->register(AndreasPabst\RequestValidation\RequestServiceProvider::class);`

Then you are able to create requests with *artisan* comparable to laravel 

## How to call

`php artisan make:request RequestName`

The new class can be found under app/Http/Requests folder.

## Example usage

Use your Request class in a controller via method injection

```php
<?php 
use App\Http\Requests\ExampleRequest;

class ExampleController extends Controller
{
    public function index(ExampleRequest $request) {
	    // ...
    }
    //...
}
```

## Other stuff...
Have Fun Using!

# Security
If you discover any security related issues, please email management@andreaspabst.com instead of using the issue tracker.

# Postcardware
You're free to use this package, but if it makes it to your product we highly appreciate you sending us a postcard from your hometown, mentioning which of our package(s) you are using.

Our address is provided on [Andreas Pabst.com](https://www.andreaspabst.com)

We publish all received postcards on our website.

# Credits
Andreas Pabst

# License
The MIT License (MIT). Please see License File for more information.