# Composer Vendor Merge

This class has the goal of automatically merge all autoload and vendor. Ideal for those who organize your project in plugins, modules, extensions, etc.

It was extracted from the OctoberCMS project core and adapted to work without the platform.

You can use this class both standalone and via composer package `composer require prhost/composer-vendor-merge`


### Example via Composer package

**Install the package**

`composer require prhost/composer-vendor-merge`

**Instance and init the classe**
```php
$manager = new Prhost\ComposerMergeVendor();
$manager->init();
```

**Adds other vendor by project**
```php
//Other vendor
$manager->addVendor(__DIR__ . '/path/to/other/vendor');
```

### Example Standalone

**Require the classe**
```php
require_once 'src/ComposerMergeVendor.php';
```

**Instance and init the classe**
```php
$manager = new Prhost\ComposerMergeVendor();
$manager->init();
```

**Adds other vendor by project**
```php
//Other vendor
$manager->addVendor(__DIR__ . '/path/to/other/vendor');
```

### Credits

* @kallefpr
* [OctoberCMS](http://octobercms.com)