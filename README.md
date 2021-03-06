# Glide

[![Author](http://img.shields.io/badge/author-@reinink-blue.svg?style=flat-square)](https://twitter.com/reinink)
[![Forked and expanded by](http://img.shields.io/badge/author-@adamale-blue.svg?style=flat-square)](https://github.com/adamale)
[![Source Code](http://img.shields.io/badge/source-adamale/glide-blue.svg?style=flat-square)](https://github.com/adamale/glide)
[![Latest Version](https://img.shields.io/github/release/adamale/glide.svg?style=flat-square)](https://github.com/adamale/glide/releases)
[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](https://github.com/adamale/glide/blob/master/LICENSE)
[![Build Status](https://img.shields.io/travis/adamale/glide/master.svg?style=flat-square)](https://travis-ci.org/adamale/glide)
[[![Total Downloads](https://img.shields.io/packagist/dt/adamale/glide.svg?style=flat-square)](https://packagist.org/packages/adamale/glide)

Glide is a wonderfully easy on-demand image manipulation library written in PHP. Its straightforward API is exposed via HTTP, similar to cloud image processing services like [Imgix](http://www.imgix.com/) and [Cloudinary](http://cloudinary.com/). Glide leverages powerful libraries like [Intervention Image](http://image.intervention.io/) (for image handling and manipulation) and [Flysystem](http://flysystem.thephpleague.com/) (for file system abstraction).

[![© Photo Joel Reynolds](https://glide.herokuapp.com/1.0/kayaks.jpg?w=1000)](https://glide.herokuapp.com/1.0/kayaks.jpg?w=1000)
> © Photo Joel Reynolds

## Highlights

- Adjust, resize and add effects to images using a simple HTTP based API.
- Manipulated images are automatically cached and served with far-future expires headers.
- Create your own image processing server or integrate Glide directly into your app.
- Supports both the [GD](http://php.net/manual/en/book.image.php) library and the [Imagick](http://php.net/manual/en/book.imagick.php) PHP extension.
- Supports many response methods, including PSR-7, HttpFoundation and more.
- Ability to secure image URLs using HTTP signatures.
- Works with many different file systems, thanks to the [Flysystem](http://flysystem.thephpleague.com/) library.
- Powered by the battle tested [Intervention Image](http://image.intervention.io/) image handling and manipulation library.
- Framework-agnostic, will work with any project.
- Composer ready and PSR-2 compliant.

## Documentation

Full documentation (except for the expanded parts) can be found at [glide.thephpleague.com](http://glide.thephpleague.com).

## Expansion

You can now keep the original image dimension (either width or height) when it is missing from the parameters by using od=1 parameter (*od* stands for *original dimension*).
It is especially useful on cropping an image, because it lets you keep one dimension intact (default behaviour is to scale the missing dimension appropriately).

```http
?w=100&od=1&fit=crop
```

## Installation

Glide is available via Composer:

```bash
$ composer require adamale/glide
```

## Testing

Glide has a [PHPUnit](https://phpunit.de/) test suite. To run the tests, run the following command from the project folder:

```bash
$ phpunit
```
## Contributing

Contributions are welcome and will be fully credited. Please see [CONTRIBUTING](https://github.com/adamale/glide/blob/master/CONTRIBUTING.md) for details.

## Security

If you discover any security related issues, please email jonathan@reinink.ca instead of using the issue tracker.

## Credits

- [Jonathan Reinink](https://github.com/reinink)
- [All Contributors](https://github.com/thephpleague/glide/contributors)
- [Adam Aleksak](https://github.com/adamale)

## License

The MIT License (MIT). Please see [LICENSE](https://github.com/adamale/glide/blob/master/LICENSE) for more information.
