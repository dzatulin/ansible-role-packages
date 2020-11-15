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
    - vim
    - htop
    - rsync
    - gzip
    - unzip
    - java
    - wget
    - git
    - nano
    remove_packages: 
    - mc
    update_packages:
    - java
  roles:
    - ansible-role-packages
```
