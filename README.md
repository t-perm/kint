# Kint - debugging helper for PHP developers

## Installation and usage
```php
<?php
require '/kint/Kint.class.php';

########## DUMP VARIABLE ###########################
Kint::dump($GLOBALS, $_SERVER); // any nuber of parameters
// or simply use d() as a shorthand:
d($_SERVER);


########## DEBUG BACKTRACE #########################
Kint::trace();
// or via shorthand:
d(1);


########## TEXT-ONLY OUTPUT ########################
s($GLOBALS);


########## MISCELLANEOUS ###########################
// to disable all output
Kint::enabled(false);
// further calls, this one included, will not yield any output
d('Get off my lawn!'); // no effect

```

### Furthermore

* `sd()` and `dd()` are shorthands for `s();die;` and `d();die;` respectively.
* `!Kint::dump()` and `!dd()` will display the dump expanded by default.

----



### Author

**Rokas Šleinius** (Raveren)

### License

Licensed under the MIT License
