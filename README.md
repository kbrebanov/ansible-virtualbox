virtualbox
==========

Installs VirtualBox.

Requirements
------------

This role requires Ansible 1.4 or higher.

Role Variables
--------------

| Name               | Default | Description                      |
|--------------------|---------|----------------------------------|
| virtualbox_version | 4.3     | Version of VirtualBox to install |

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
