
# OnrampLab's PHPCS Configuration

We use this package to set up a consistent PHPCS configuration across my Laravel projects. The ruleset is based on [@emielmolenaar ruleset](https://github.com/emielmolenaar/onr-phpcs-laravel).

If you wish to use this configuration in your project, install it using composer:

`composer require --dev onramplab/phpcs-laravel`

Afterwards, run `php vendor/bin/phpcs -i` to verify that `onr-phpcs-laravel` is listed as an installed ruleset.

You may now use the ruleset like so:

`php vendor/bin/phpcs --standard=onr-phpcs-laravel app/`

Or you can create a `phpcs.xml` file in your root folder with following example:

```xml
<?xml version="1.0"?>
<ruleset name="Onramplab Laravel Standards">

    <description>The Laravel Coding Standards</description>

    <rule ref="onr-phpcs-laravel"/>

    <file>app</file>
    <file>config</file>
    <file>public</file>
    <file>resources</file>
    <file>routes</file>
    <file>tests</file>

</ruleset>
```

Contributions welcome.
