# Generator

Laravel starter app and simple CRUD generator.

## Requirements

- PHP ^8.2
- Laravel with package auto-discovery enabled
- yajra/laravel-datatables-oracle (^11.0 or ^12.0)

## Installation

```bash
composer require in-sohel-rana/generator
```

### Install preset

Full version (requires `laravel/fortify` and `spatie/laravel-permission`):

```bash
composer require laravel/fortify spatie/laravel-permission
php artisan generator:install full
```

Simple version:

```bash
php artisan generator:install simple
```

## Artisan commands

- `php artisan generator:install {full|simple}`: publish required files for the selected preset.
- `php artisan generator:publish-api`: publish API routes, requests, and controllers.
- `php artisan generator:publish-utils`: publish utility classes.
- `php artisan generator:publish-image-service-v2`: publish the image service v2 classes.
- `php artisan generator:sidebar {static|dynamic}`: switch sidebar rendering mode.

## Publish tags

Use `php artisan vendor:publish --tag=<tag> --force` for specific resources.

- `generator-view`
- `generator-config`
- `generator-config-simple`
- `generator-controller`
- `generator-request-role`
- `generator-request-user`
- `generator-request-api`
- `generator-controller-api`
- `generator-role-user-resource-api`
- `generator-action`
- `generator-provider`
- `generator-view-provider`
- `generator-migration`
- `generator-seeder`
- `generator-model`
- `generator-assets`
- `generator-utils`
- `image-service-v2`
- `bootstrap-app-full`
- `bootstrap-app-simple`

## Development

```bash
composer lint
composer test
```

## Docs and links

- Source: https://github.com/in-sohel-rana/generator
