Role Name
=========

Installs VirtualBox.

Requirements
------------

This role requires Ansible 1.4 or higher.

Role Variables
--------------

    # VirtualBox version to install
    virtualbox_version: 4.3

Dependencies
------------

Example Playbook
----------------

1) Install VirtualBox

    - hosts: all
      roles:
         - { role: virtualbox }

2) Install specific version of VirtualBox

    - hosts: all
      roles:
         - { role: virtualbox, virtualbox_version: 4.1 }

License
-------

BSD

Author Information
------------------

Kevin Brebanov
