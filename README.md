# Ansible Role: phpMyAdmin

An Ansible role that installs phpMyAdmin on Ubuntu.

## Requirements

For the configuration with nginx the directories for sites must already exist (e.g. nginx has to be installed).

## Role Variables

Available variables are listed below, along with default values:

    phpmyadmin_web_server: nginx
    phpmyadmin_php_fpm_socket: localhost:9000

    phpmyadmin_server_host: localhost
    phpmyadmin_server_auth_type: config
    phpmyadmin_server_user: root
    phpmyadmin_server_password: root

## Dependencies

None

## Example Playbook

    - hosts: all
      roles:
        - { role: mjanser.phpmyadmin }

## License

MIT
