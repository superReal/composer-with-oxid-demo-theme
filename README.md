composer-with-oxid-demo-theme
===============

Demo theme for showing how to handle OXID themes with composer

Installation
======

1. Define this repository as requirement in your projects root composer.json
2. Put all your assets to the skin directory, this will be symlinked to the out folder
3. Put the following scripts to your projects root composer.json, to symlink the assets to the out folder
```
    "scripts": {
        "post-autoload-dump": [
            "ln -sf ../application/views/composer-with-oxid-demo-theme/skin/composer-with-oxid-demo-theme out/composer-with-oxid-demo-theme"
        ]
    }
```
