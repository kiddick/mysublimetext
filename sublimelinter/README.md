It is possible to specofy linter settings per project.

So edit project settings with:

```
    "SublimeLinter":
    {
        "@python": 3,
        "linters": {
            "pylint": {
                "@disable": false,
                "args": [
                    "--max-line-length=120",
                ],
                "enable": "",
                "excludes": [],
                "jobs": 4,
                "paths": [],
                "rcfile": "",
                "show-codes": true
            },
            "pep8": {
                "@disable": true,
            },
            "pycodestyle": {
                "@disable": true,
            },
            "pyflakes": {
                "@disable": true,
            }
        },

    }
```

Add desired options to separate root level section `SublimeLinter`.

To specify python version use `@python`.

Note that only meta-settings(http://www.sublimelinter.com/en/latest/settings.html#meta) and linter(http://www.sublimelinter.com/en/latest/settings.html#linter) settings are recognized in project settings.


To disable specific errors and warnings use `--disable` cli argument:
```
"args": [
    "--disable=W0613"
],
```
