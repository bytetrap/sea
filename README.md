# sea

<a href="https://github.com/bytetrap/sea">
    <img src="sea.png" width="80" height="80" align="right">
</a>

> Start here.

[![build][build-image]][build-url]
[![version][version-image]][version-url]
[![license][license-image]][license-url]

## Installation

**Git**

```
git clone https://github.com/bytetrap/sea.git
```

To do this, please install dependencies with `Composer` first.

```
composer install
```

Copy the `.env.example` file and rename it to `.env`, configure database connection in `.env` file, then generate the new key to `.env` file.

```
php artisan key:generate --ansi
```

Finally, run the following command to publish resources, and complete the installation.

```
php artisan vendor:publish --provider="Encore\Admin\AdminServiceProvider"
php artisan admin:install
```

**Composer**

```
composer create-project bytetrap/sea
```

Then configure database connection in `.env` file, and run the following command.

```
php artisan admin:install
```

## How to use it?

After starting the service, open [http://localhost/admin/](http://localhost/admin/) in the browser, and log in with the username `admin` and password `admin` .

## License

`sea` is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT) .



[build-image]: https://img.shields.io/badge/build-passing-brightgreen   "build"
[build-url]: https://github.com/bytetrap/sea "build"
[version-image]: https://img.shields.io/badge/version-v1.0.4-blue   "version"
[version-url]: https://github.com/bytetrap/sea   "version"
[license-image]: https://img.shields.io/badge/license-MIT-green "license"
[license-url]: https://opensource.org/licenses/MIT  "license"