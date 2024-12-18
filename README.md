# modanisa/iyzipay-php

This is copy of [iyzico/iyzipay-php](https://github.com/iyzico/iyzipay-php) with some modifications to make it work with PHP 7.2+ rather than PHP 7.4+

## Modifications

- Removed type declarations from class properties
- Downgrade PHPUnit to 8
- Prepend `modanisa/` to `x-iyzi-client-version` header

## How to use this package instead of iyzico/iyzipay-php

In your project composer.json file, add the following repository:

```json
{
    "repositories": [
        {
            "type": "github",
            "url": "git@github.com:modanisa/iyzipay-php.git"
        }
    ]
}
```

Then, change the version of iyzico/iyzipay-php to `dev-master` (without changing the name):

```json
{
    "require": {
        "iyzico/iyzipay-php": "dev-master"
    }
}
```

Finally, run `composer update` to update the package.
