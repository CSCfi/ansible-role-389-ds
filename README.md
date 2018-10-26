[![Build Status](https://travis-ci.org/CSCfi/ansible-role-389-ds.svg?branch=master)](https://travis-ci.org/CSCfi/ansible-role-389-ds)

# Ansible-Role: 389-ds

An role which install 389 Directory Server on RedHat/Debian servers.

### Requirements

None

### Dependencies

None


## Role Variables

See defaults/main.yml for the variables you can overwrite via role call as a parameter.

| Variable | Purpose |
| :------- | :------ |
| `dirsrv_password` | Password, **be sure to set** |
| `dirsrv_admin_password` | Admin password ( Default: dirsrv_password ) |
| `dirsrv_fqdn` | FQDN  (Default: ansible_fqdn, if ansible_fqdn fails or is wrong for you, set proper one )|
| `dirsrv_suffix` | Default: last two parts from dirsrv_fqdn |
| `dirsrv_hostname` | Default: first part from dirsrv_fqdn |


## Example playbook

    - hosts: all
      roles:
        - CSCfi.389-ds 
