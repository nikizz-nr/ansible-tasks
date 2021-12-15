#Ansible role: install_vsftpd

Installs and configures vsftpd

Requirements
------------

None

Role Variables
--------------

Used in vsftpd.conf:
anonymous_enable: "YES"
write_enable: "YES"
anon_upload_enable: "YES"
anon_mkdir_write_enable: "YES"
anon_root: "/var/ftp/pub/"
listen: "YES"
anon_umask: "022"

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - install_vsftpd

License
-------

BSD

Author Information
------------------

Nikita Rubtsov <Nikita_Rubtsov@epam.com>
