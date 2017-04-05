[![Build Status](https://travis-ci.org/CSC-IT-Center-for-Science/ansible-role-apache.svg?branch=master)](https://travis-ci.org/CSC-IT-Center-for-Science/ansible-role-apache)

Ansible-Role: 389-ds
=========

An role which install 389 Directory Server on RedHat/Debian servers.
Purpose of this role is to perform base installation

Requirements
------------

None.

Role Variables
--------------

See defaults/main.yml for the variables you can overwrite via role call as a parameter.

* dirsrv_state: latest

Dependencies
------------

None

Example Playbook
----------------

    - hosts: ldapserver
      roles:
        - { role: CSCfi.389-ds }
