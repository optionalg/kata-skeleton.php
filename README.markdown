## Usage

Those usages assume that your are using the CLI. You can of course use this skeleton with any IDE.

Clone the repository on your local machine:

```bash
$ git clone https://github.com/kevinlebrun/kata-skeleton.php.git
$ cd /path/to/kata-skeleton.php
$ rm -rf .git
```

It is a good idea to rename your Kata directory with a more meaningful name.

Edit the `composer.json` file with your requirements then run in console:

```bash
$ cd /path/to/kata/directory
$ curl -s http://getcomposer.org/installer | php
$ ./composer.phar install --dev
```

If you keep PHPUnit, you can use it from the CLI:

```bash
$ ./bin/phpunit
```

Don't forget to update the `composer.json` file with autoloader configuration:

```json
"autoload": {
    "psr-0": {
        "YourNamespace": "src"
    }
}
```

Then you should regenerate autoloading informations with Composer:

```bash
$ ./composer.phar dump-autoload
```

You can go further by reading the "Getting Started" section of Composer [here](http://getcomposer.org/doc/00-intro.md "Composer introduction").

The use of any versionning tool during your Kata is highly encouraged.
