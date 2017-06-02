# Supported tags and respective ```Dockerfile``` links
* ```latest```
* ```alpine```

**This is a Dockerised Solution for running PHPCS with CakePHP Standards**.

## What is PHPCS?

PHP_CodeSniffer is a set of two PHP scripts; the main ```phpcs``` script that tokenizes PHP, JavaScript and CSS files to detect violations of a defined coding standard, and a second ```phpcbf``` script to automatically correct coding standard violations. PHP_CodeSniffer is an essential development tool that ensures your code remains clean and consistent.

## What are CakePHP Coding Standards?

The [CakePHP Coding Standards](https://book.cakephp.org/2.0/en/contributing/cakephp-coding-conventions.html) apply to code within CakePHP.

## Docker Commands

### Pull

```
docker pull willhallonline/cakephp-phpcs
docker pull willhallonline/cakephp-phpcs:alpine
```

### Run

#### PHPCS (PHP CodeSniffer)

```
docker run -it --rm -v $(pwd):/app willhallonline/cakephp-phpcs phpcs [YOUR-CODE]
docker run -it --rm -v $(pwd):/app willhallonline/cakephp-phpcs:alpine phpcs [YOUR-CODE]
```

#### PHPCBF (PHP CodeFixer)

```
docker run -it --rm -v $(pwd):/app willhallonline/cakephp-phpcs phpcbf [YOUR-CODE]
docker run -it --rm -v $(pwd):/app willhallonline/cakephp-phpcs:alpine phpcbf [YOUR-CODE]
```
