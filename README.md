# Ansible Role: MariaDB

[![Build Status](https://travis-ci.org/tschifftner/ansible-role-mariadb.svg)](https://travis-ci.org/tschifftner/ansible-role-mariadb)

Installs MariaDB on Debian/Ubuntu linux servers.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

### Security

This role sets an administrative user and removes root entirely. Please define the following settings:

```
mariadb_admin_home: '/root'
mariadb_admin_user: 'admin'
mariadb_admin_password: 'Set strong password here!'
```

## Dependencies

None.

## Example Playbook

    - hosts: server
      roles:
        - { role: tschifftner.mariadb }

## Supported OS
Ansible          | Debian Jessie    | Ubuntu 14.04    | Ubuntu 12.04
:--------------: | :--------------: | :-------------: | :-------------: 
1.8              | Yes              | Yes             | Yes
1.9              | Yes              | Yes             | Yes

## License

MIT / BSD

## Author Information

 - Tobias Schifftner, @tschifftner