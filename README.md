# Laravel Basic Authentication

Simple package to add Basic Authentication / BA to your Laravel project with 4 easy steps.

# Step 1. Install
##### Install with composer
```
$ composer require redcenter/laravel-basic-authentication
```

# Step 2. Adding middleware
Add the middleware class to your Kernel.php in App\Http:
```
    protected $middleware = [
        ...
        LaravelBasicAuth::class,
        ...
        ],
    ];
```

# Step 3. Adding env variables
Add the variables to your .env file
```
AUTH_BASIC_USER=your-user-name
AUTH_BASIC_PASSWORD=your-password
```

# Step 4. Loading env variables in your config
Load the env variables through your config file in config/app.php
```
return [
    ...
    'basic_auth_user' => env('AUTH_BASIC_USER', null),
    'basic_auth_password' => env('AUTH_BASIC_PASSWORD', null),
    ...
]
```

# Open your project
Now, when you open your project in the browser, you will need the credentials to proceed.

Do you want to disable the BA middleware? Delete the variables from your .env (or delete the values)... That's it.

## Questions?
You can contact me through my website: redcenter.nl

##### Good bye!

Check out the documentation on Bitbucket for all details!

https://bitbucket.org/redcenter/laravel-basic-authentication
