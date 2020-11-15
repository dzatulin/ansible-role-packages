# Ansible Packages Role
Role for installing, removing and updating packages
## Requirements
Ansible version: 2.9
Centos 7/ Debian
## Dependencies
None
## Example Playbook
```
- name: update
  hosts: "{{ var }}"
  vars:
    install_all_package_updates: false
    install_packages:
    - epel-release
    - mc
    - vim
    - htop
    - rsync
    - gzip
    - unzip
    - java
    - wget
    - git
    - nano
  roles:
    - ansible-role-packages
```
