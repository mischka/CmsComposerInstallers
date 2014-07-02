composer-installers
===================


How to use
==========

```json
{
  "repositories": [
    {
      "type": "composer",
      "url": "http://composer.typo3.org/"
    }
  ]
}
```

Notice:
-------

Extensions with ext-keys containing underscores are equivalent to packages with minus so "extension_builder" to "typo3-ter/extension-builder"


Example:
--------
```json
{
    "name": "foo/bar",
    "description": "foo bar",
    "license": "",
    "authors": [
        {
            "name": "John Doe",
            "email": "foo@bar.buzz"
        }
    ],
    "repositories": [
        {
            "type": "composer",
            "url": "http://composer.typo3.org/"
        }
    ],
    "minimum-stability": "dev",
    "require": {
        "typo3/cms": "~6.2",

        "typo3-ter/formhandler": "~2.0.0",
        "typo3-ter/cooluri": "~1.0.37",

        "typo3-ter/flux": "*",
        "typo3-ter/vhs": "*",
        "typo3-ter/fluidcontent": "*",
        "typo3-ter/fluidpages": "*"

    },
    "require-dev": {
        "typo3-ter/extension-builder": "~6.2.0"
    },
    "extra": {
        "typo3-cms-web-dir": "htdocs",
        "typo3-cms-core-installer-path": "htdocs/typo3_src",
        "typo3-cms-extension-installer-path": "htdocs/typo3conf/ext"
    }
}
```