# Ansible Role: PHP Versions Cohabitat

Based on v7.0.0 of [Jeff Geerling's PHP Versions Ansible role](https://github.com/geerlingguy/ansible-role-php-versions) created in 2017 by [Jeff Geerling](https://www.jeffgeerling.com/), author of [Ansible for DevOps](https://www.ansiblefordevops.com/).

## Purpose of this fork

Forked to make the purging action of other PHP versions an optional task, controllable via the boolean variable 
`keep_one_php_version_only` , since [Jeff wants to keep this purging behaviour in his role as is](https://github.com/geerlingguy/ansible-role-php-versions/issues/85).


By default, `keep_one_php_version_only` is set to `false`; means this role won't purge other PHP versions already installed on the server.

Hence the name Cohabitat!

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    php_version: '8.3'
    keep_one_php_version_only: false

## License

MIT / BSD

## Full Documentation

Available at [Jeff Geerling's PHP Versions Ansible role repo](https://github.com/geerlingguy/ansible-role-php-versions) 
