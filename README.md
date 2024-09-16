# Pimcore Ntriga Cookies

Package to handle cookies for Ntriga projects

### Dependencies

| Release  | Supported Pimcore Versions | Supported Symfony Versions | Maintained     | Branch |
|----------|----------------------------|----------------------------|----------------|--------|
| **11.x** | `11.0`                     | `6.2`                      | Feature Branch | master |

## Installation

You can install the package via composer:

```bash
composer require ntriga/pimcore-ntriga-cookies
```

Add Bundle to `bundles.php`:

```php
return [
    Ntriga\PimcoreCookies\PimcoreNtrigaCookiesBundle::class => ['all' => true],
];
```
## Usage

Add to include before the closing body tag in your layout template:
    
```twig
{% include '@PimcoreNtrigaCookies/cookies.html.twig' %}
```
When we don't want to set Analytical Cookies, we can pass a parameter
```
{% include '@PimcoreNtrigaCookies/cookies.html.twig' with {'AnalyticalCookies': 'false'} %}
```

## Changelog
Please see [CHANGELOG](CHANGELOG.md) for more information on what has changed recently.

## Credits
- [All contributors](../../contributors)

## License
GNU General Public License version 3 (GPLv3). Please see [License File](./LICENSE.md) for more information.

