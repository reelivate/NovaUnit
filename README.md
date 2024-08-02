# NovaUnit

[![Latest Version on Packagist](https://img.shields.io/packagist/v/jamesfreeman/novaunit.svg?style=flat-square)](https://packagist.org/packages/joshgaber/novaunit)
[![Total Downloads](https://img.shields.io/packagist/dt/jamesfreeman/novaunit.svg?style=flat-square)](https://packagist.org/packages/jamesfreeman/novaunit)

[NovaUnit](https://jamesfreeman.github.io/NovaUnit) is a unit-testing package for Laravel Nova, built using PHPUnit. NovaUnit provides you with assertions for Nova Actions, Lenses and Resources, so you can create great administration panels with confidence.

## Installation

You can install the package in your Laravel Project via composer:

```sh
composer require --dev jamesfreeman/novaunit
```

### Requirements

* PHP 8.0 or higher
* [Laravel](https://laravel.com/) 6.x - 11.x
* [Laravel Nova](https://nova.laravel.com/) 2.x - 4.x
* [PHPUnit](https://github.com/sebastianbergmann/phpunit) 8.5.x - 11.x

## Usage

To access the test classes, import and use the base test traits:

```php
class ClearLogsTest extends TestCase {
    use NovaActionTest;
}
```

Once you've created the mock with the initial test class, you can begin testing different aspect of the component:

```php
$this->novaAction(ClearLogs::class)
    ->assertHasField('since_date');
```

For a list of available methods, see the [full docs site](https://jamesfreeman.github.io/NovaUnit).

### Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information what has changed recently.

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

### Security

If you discover any security related issues, please email github@james-freeman.info instead of using the issue tracker.

## Created By

* [Josh Gaber](https://github.com/joshgaber) (Creator)
* [James Freeman](https://github.com/jamesfremean) (Maintainer)

## Contributors

* [Joshua Lauwrich Nandy](https://github.com/joshua060198)
* [nicko170](https://github.com/nicko170)
* [Henry Ávila](https://github.com/henryavila)
* [Peter Elmered](https://github.com/pelmered)

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.

## Laravel Package Boilerplate

This package was generated using the [Laravel Package Boilerplate](https://laravelpackageboilerplate.com).
