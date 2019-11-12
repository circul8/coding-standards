# Circul8 Coding Standards
Circul8 coding standards and dot files.

## Installation

### Install Slevomat Coding Standards
```php
composer require slevomat/coding-standard --dev
```

### Edit `composer.json`

Add two scripts there, `lint` & `lintfix`:

```json
{
  "require-dev": {
    "slevomat/coding-standard": "^5.0"
  },
  "scripts": {
    "lint": [
      "vendor/bin/phpcs --standard=ruleset.xml"
    ],
    "lintfix": [
      "vendor/bin/phpcbf --standard=ruleset.xml"
    ]
  }
}
```

### Download `ruleset.xml` and `.editorconfig`
```sh
wget -nv https://raw.githubusercontent.com/circul8/coding-standards/master/.editorconfig
wget -nv https://raw.githubusercontent.com/circul8/coding-standards/master/phpcs.xml
```

Edit `ruleset.xml` if necessary.
