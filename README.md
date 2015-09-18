consul
=======

[![Ansible Role](https://img.shields.io/ansible/role/3300.svg)](https://galaxy.ansible.com/list#/roles/3300)

Installs Consul

Requirements
------------

This role requires Ansible 1.4 or higher.

Role Variables
--------------

| Name             | Default                                                          | Description                  |
|------------------|------------------------------------------------------------------|------------------------------|
| consul_version   | 0.5.2                                                            | Version of Consul to install |
| consul_sha256sum | 171cf4074bfca3b1e46112105738985783f19c47f4408377241b868affa9d445 | SHA 256 checksum of package  |

Dependencies
------------

- kbrebanov.unzip

Example Playbook
----------------

Install Consul
```
- hosts: all
  roles:
    - { role: kbrebanov.consul }
```

Install Consul specifying version and checksum
```
- hosts: all
  roles:
    - { role: kbrebanov.consul, consul_version: 0.4.1, consul_sha256sum: 2cf6e59edf348c3094c721eb77436e8c789afa2c35e6e3123a804edfeb1744ac }
```

License
-------

BSD

Author Information
------------------

Kevin Brebanov
