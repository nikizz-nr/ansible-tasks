#Ansible role: install_httpd

Installs https and creates simple index file.

Requirements
------------

None

Role Variables
--------------

Service name
service_name: httpd

Serivice name in systemd
service_full_name: httpd.service

Path to index page
index_page_path: /var/www/html/index.html

Index page template
index_file_template: index.j2

Web server user
httpd_user: apache

Firewall service to enable
firewall_service: http

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - install_httpd

License
-------

BSD

Author Information
------------------

Nikita Rubtsov <Nikita_Rubtsov@epam.com>
