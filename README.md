[![No Maintenance Intended](http://unmaintained.tech/badge.svg)](http://unmaintained.tech/)

virtualbox
==========

[![Ansible Role](https://img.shields.io/ansible/role/3310.svg)](https://galaxy.ansible.com/list#/roles/3310)

Installs VirtualBox.

Requirements
------------

This role requires Ansible 1.4 or higher.

Role Variables
--------------

| Name               | Default | Description                      |
|--------------------|---------|----------------------------------|
| virtualbox_version | 5.0     | Version of VirtualBox to install |

Dependencies
------------

CentOS:
  - kbrebanov.selinux
  - kbrebanov.dkms
  - kbrebanov.kernel_headers

Ubuntu:
  - kbrebanov.dkms
  - kbrebanov.kernel_headers

Example Playbook
----------------

Install VirtualBox
```
- hosts: all
  roles:
    - { role: kbrebanov.virtualbox }
```

Install specific version of VirtualBox
```
- hosts: all
  roles:
    - { role: kbrebanov.virtualbox, virtualbox_version: 4.2 }
```

License
-------

BSD

Author Information
------------------

Kevin Brebanov
