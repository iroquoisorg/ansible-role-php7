# php7

[![Build Status](https://travis-ci.com/iroquoisorg/ansible-role-php7.svg?branch=master)](https://travis-ci.com/iroquoisorg/ansible-role-php7)

Ansible role for php7

This role was prepared and tested for Ubuntu 16.04.

# Installation

`$ ansible-galaxy install iroquoisorg.php7`

# Default settings

```
---
php7_version: "{{ php_version | default('7.2') }}"

php_extensions:
  - "php{{ php7_version }}-cli"
  - "php{{ php7_version }}-gd"
  - "php{{ php7_version }}-pgsql"
  - "php{{ php7_version }}-mongodb"
  - "php{{ php7_version }}-memcached"
  - "php{{ php7_version }}-curl"
  - "php{{ php7_version }}-intl"
  - "php{{ php7_version }}-dev"
  - "php{{ php7_version }}-xml"
  - "php{{ php7_version }}-mbstring"
  - "php{{ php7_version }}-bcmath"
  - "php{{ php7_version }}-fpm"
  - php-pear

php_http_connector: apache  # fpm or apache

php_ini_lines: []

```

# Development

Please check [development guide](DEVELOPMENT.md) for details about developing and testing this role.
