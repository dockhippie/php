# PHP Nginx

[![](https://images.microbadger.com/badges/image/webhippie/php-nginx.svg)](https://microbadger.com/images/webhippie/php-nginx "Get your own image badge on microbadger.com")

These are docker images for [PHP](https://secure.php.net) running on a [Nginx container](https://registry.hub.docker.com/u/webhippie/nginx/).


## Versions

* [latest](https://github.com/dockhippie/php/tree/master/nginx) available as ```webhippie/php-nginx:latest``` at [Docker Hub](https://registry.hub.docker.com/u/webhippie/php-nginx/)
* [7](https://github.com/dockhippie/php/tree/7/nginx) available as ```webhippie/php-nginx:7``` at [Docker Hub](https://registry.hub.docker.com/u/webhippie/php-nginx/)
* [5](https://github.com/dockhippie/php/tree/5/nginx) available as ```webhippie/php-nginx:5``` at [Docker Hub](https://registry.hub.docker.com/u/webhippie/php-nginx/)


## Volumes

* /srv/www
* /etc/php5/custom.d


## Ports

* 8080


## Available environment variables

```bash
ENV PHP_MEMORY_LIMIT 512M
ENV PHP_ERROR_LOG /proc/self/fd/2
ENV PHP_ERROR_REPORTING E_ALL & ~E_DEPRECATED & ~E_STRICT
ENV PHP_DISPLAY_ERRORS On
ENV PHP_DISPLAY_STARTUP_ERRORS On
ENV PHP_LOG_ERRORS On
ENV PHP_LOG_ERRORS_MAX_LEN 1024
ENV PHP_IGNORE_REPEATED_ERRORS Off
ENV PHP_IGNORE_REPEATED_SOURCE Off
ENV PHP_REPORT_MEMLEAKS On
ENV PHP_TRACK_ERRORS Off
ENV PHP_HTML_ERRORS On
ENV PHP_POST_MAX_SIZE 2G
ENV PHP_UPLOAD_MAX_FILESIZE 2G
ENV PHP_MAX_EXECUTION_TIME 3600
ENV PHP_MAX_INPUT_TIME 3600
ENV PHP_DATE_TIMEZONE UTC
ENV PHP_LOG_LEVEL warning
ENV PHP_MAX_CHILDREN 75
ENV PHP_MAX_REQUESTS 500
ENV PHP_PROCESS_IDLE_TIMEOUT 10s
ENV PHP_COMPOSER_INSTALL true
```


## Inherited environment variables

* [webhippie/nginx](https://github.com/dockhippie/nginx#available-environment-variables)
* [webhippie/alpine](https://github.com/dockhippie/alpine#available-environment-variables)


## Contributing

Fork -> Patch -> Push -> Pull Request


## Authors

* [Thomas Boerger](https://github.com/tboerger)
* [Christoph Wiechert](https://github.com/psi-4ward)


## License

MIT


## Copyright

```
Copyright (c) 2015-2017 Thomas Boerger <http://www.webhippie.de>
```
