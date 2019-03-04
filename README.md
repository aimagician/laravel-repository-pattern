[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/mshamaseen/laravel-repository-pattern/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/mshamaseen/laravel-repository-pattern/?branch=master)
[![Code Coverage](https://scrutinizer-ci.com/g/mshamaseen/laravel-repository-pattern/badges/coverage.png?b=master)](https://scrutinizer-ci.com/g/mshamaseen/laravel-repository-pattern/?branch=master)
[![Build Status](https://scrutinizer-ci.com/g/mshamaseen/laravel-repository-pattern/badges/build.png?b=master)](https://scrutinizer-ci.com/g/mshamaseen/laravel-repository-pattern/build-status/master)
[![Code Intelligence Status](https://scrutinizer-ci.com/g/mshamaseen/laravel-repository-pattern/badges/code-intelligence.svg?b=master)](https://scrutinizer-ci.com/code-intelligence)
[![SymfonyInsight](https://insight.symfony.com/projects/f3edab7d-00b8-4633-96d3-a84e38b7ebec/mini.svg)](https://insight.symfony.com/projects/f3edab7d-00b8-4633-96d3-a84e38b7ebec)
# Repository Generator
Autogeneration for repository pattern files, This package is aim to generate Contract (interface), Entity (model), Controller, Repository and Request validation files for specified module.

*Note: if you are using laravel, you should've at least version **5.7**

## Requirement

This package require the following dependencies:
   "illuminate/console": "^5.7",
   "illuminate/support": "^5.7"

## Install

1- Require this package with composer using the following command:
```bash
composer require --dev shamaseen/repository-generator
```
2- publish the package config file by running:
```bash
php artisan vendor:publish
```
and select **repository-config**.

Note: this package is aim to be only for development environment.

## Publish stubs
If you want to have a custom stubs rather than the default ones, you can change the path of the stubs folder in repository config, then run the following command:
```bash
php artisan vendor:publish
```

and select **repository-stub**, this will publish all the stub templates to the specified path on repository config.
Feel free to edit stubs templates.

## How to use
To generate repository files run the following command:
```bash
php artisan make:repository {Folder/Classname (singular)}
```
where Folder is optional.

## Examples

To generate repository files for product, run the following:

```bash
php artisan make:repository Products/Product
```
Note: You can use Product instead of Products/Product, this will not make new folder with the class.


## License
Repository-generator is a free software distributed under the terms of the MIT license.
