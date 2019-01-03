# Ansible Role: install nginx

Ansible Role: Install nginx

## Requirements

OS: Ubuntu16.04
php and python are installed before this.

## Getting started

```
$ ansible_galaxy install gano2018.ansible_nginx --roles-path <your_roles_directory>
```

## Role Variables

- nginx_document_root

  This is the location of document root, whose default value is `/home/doc_root`

- nginx_php_fpm_version

  This is the version for php suitable fpm, whose default value is `7.0`
  If you use php7, you must specify 7.0, then you will use php7.0-fpm.

- nginx_service_port

  This is the port the nginx uses. The default value is `80`

- nginx_vhost_conf

  This is the location where the nginx conf file is stored.

- nginx_packages

  This is the needed packages when installed nginx.
  The default value is `nginx` and `php{{ nginx_php_fpm_version }}-fpm`
