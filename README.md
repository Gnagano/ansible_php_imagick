# Ansible Role: build imagick from the source for php use

This ansible roles allow you to install imagick and set it for php.

## Requirements

OS: Ubuntu16.04
PHP: version >= 7.0

## Getting started

```
$ ansible_galaxy install Gnagano.ansible_php_imagick --roles-path <your_roles_directory>
```

## Role Variables 

- imagick_download_dir (edit required)

  This variable is the destination for git clone imagick.git. The default value is `/tmp/imagick`

- imagick_repository

  The [url of repository](https://github.com/mkoppanen/imagick) for imagick.git
  

- imagick_packages

  The required packages to install imagick.
