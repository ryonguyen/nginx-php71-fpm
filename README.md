[![Docker Hub; wyveo/nginx-php-fpm](https://img.shields.io/badge/docker%20hub-wyveo%2Fnginx--php--fpm-blue.svg?&logo=docker&style=for-the-badge)](https://hub.docker.com/r/wyveo/nginx-php-fpm/) [![](https://img.shields.io/microbadger/image-size/wyveo/nginx-php-fpm/php71.svg?&style=for-the-badge)](https://microbadger.com/images/wyveo/nginx-php-fpm) [![](https://img.shields.io/microbadger/layers/wyveo/nginx-php-fpm/php71.svg?&style=for-the-badge)](https://microbadger.com/images/wyveo/nginx-php-fpm) [![nginx 1.15.12](https://img.shields.io/badge/nginx-1.15.12-brightgreen.svg?&logo=nginx&logoColor=white&style=for-the-badge)](https://nginx.org/en/CHANGES) [![php 7.1.29](https://img.shields.io/badge/php--fpm-7.1.29-blue.svg?&logo=php&logoColor=white&style=for-the-badge)](https://secure.php.net/releases/7_1_29.php) [![License MIT](https://img.shields.io/badge/license-MIT-blue.svg?&style=for-the-badge)](https://github.com/wyveo/nginx-php-fpm/blob/master/LICENSE)

## Introduction
This is a Dockerfile to build a debian based container image running nginx and php-fpm 7.3.x / 7.2.x / 7.1.x / 7.0.x & Composer

### Versioning
| Docker Tag | GitHub Release | Nginx Version | PHP Version | Debian Version |
|-----|-------|-----|--------|--------|
| latest | master Branch |1.15.12 | 7.3.5 | stretch |
| php73 | php73 Branch |1.15.12 | 7.3.5 | stretch |
| php72 | php72 Branch |1.15.12 | 7.2.18 | stretch |
| php71 | php71 Branch |1.15.12 | 7.1.29 | stretch |
| php70 | php70 Branch |1.15.12 | 7.0.33 | stretch |

## Building from source
To build from source you need to clone the git repo and run docker build:
```
$ git clone https://github.com/ryonguyen/nginx-php-fpm.git
```

followed by
```
$ docker build -t nginx-php-fpm:php71 . # PHP 7.1.x
```

## Pulling from Docker Hub
```
$ docker pull ryonguyen/nginx-php-fpm:latest
```

## Running
To run the container:
```
$ sudo docker run -d ryonguyen/nginx-php-fpm:latest
```

Default web root:
```
/usr/share/nginx/html
```
