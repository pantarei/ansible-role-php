Ansible Role for PHP
====================

[![Build Status](https://travis-ci.org/pantarei/ansible-role-php.svg?branch=master)](https://travis-ci.org/pantarei/ansible-role-php)
 [![GitHub tag](https://img.shields.io/github/tag/pantarei/ansible-role-php.svg)](https://github.com/pantarei/ansible-role-php)
 [![GitHub license](https://img.shields.io/github/license/pantarei/ansible-role-php.svg)](https://github.com/pantarei/ansible-role-php/blob/master/LICENSE)
 [![Ansible Role](https://img.shields.io/ansible/role/6354.svg)](https://galaxy.ansible.com/detail#/role/6354)

Ansible Role for PHP Installation.

Requirements
------------

This role require Ansible 1.9 or higher.

This role was designed for Ubuntu Server 14.04 LTS.

Role Variables
--------------

No additional role variables.

Dependencies
------------

-   [hswong3i.apt](https://github.com/pantarei/ansible-role-apt)

Example Playbook
----------------

    - hosts: servers
      roles:
        - { role: hswong3i.php }

License
-------

-   Code released under [MIT](https://github.com/pantarei/ansible-role-php/blob/master/LICENSE)
-   Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

Author Information
------------------

-   Wong Hoi Sing Edison
    -   <https://twitter.com/hswong3i>
    -   <https://github.com/hswong3i>

