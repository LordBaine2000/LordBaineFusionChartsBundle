FusionCharts Bundle for Symfony2

## Current Version

FusionCharts XT (v3.3.1 - Service Release 2)

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
        // ...
        "lordbaine/fusion-charts-bundle": "dev-master"
    }
}
```

### Add bundle to your application kernel

``` php
// app/AppKernel.php

public function registerBundles()
{
    $bundles = array(
        // ...
        new LordBaine\FusionChartsBundle\LordBaineFusionChartsBundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update lordbaine/fusion-charts-bundle
```

### Install assets

Given your server's public directory is named "web", install the public vendor resources

``` bash
$ php app/console assets:install web
```

Optionally, use the --symlink attribute to create links rather than copies of the resources 

``` bash
$ php app/console assets:install --symlink web
```

## Usage

Refer to the desired files in your HTML template, e.g.

``` html
{% javascripts '@LordBaineFusionChartsBundle/Resources/public/js/FusionCharts.js' %}
    <script type="text/javascript" src="{{ asset_url }}"></script>
{% endjavascripts %}
```

## Licenses

Refer to the source code of the included files for license information

## References

1. http://www.fusioncharts.com/products/suite/fusioncharts-xt/
2. http://symfony.com
