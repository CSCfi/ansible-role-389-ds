[![Build Status](https://travis-ci.org/CSC-IT-Center-for-Science/ansible-role-apache.svg?branch=master)](https://travis-ci.org/CSC-IT-Center-for-Science/ansible-role-apache)

Ansible-Role: 389-ds
=========

An role which install 389 Directory Server on RedHat/Debian servers.

Requirements
------------

None

Role Variables
--------------

See defaults/main.yml for the variables you can overwrite via role call as a parameter.

* dirsrv_state: latest
* dirsrv_password: PLEASE SET
* dirsrv_admin_password: ( Default: dirsrv_password )

* dirsrv_fqdn: ( Default: ansible_fqdn, if ansible_fqdn fails or is wrong for you, set proper one )
* dirsrv_suffix: ( Default: last two parts from dirsrv_fqdn )
* dirsrv_hostname: ( Default: first part from dirsrv_fqdn )

Dependencies
------------

None

Example Playbook
----------------

    - hosts: ldapserver
      roles:
        - { role: CSCfi.389-ds }
