# Ansible Packages Role
Role for installing, removing and updating packages
## Requirements
Ansible version: 2.9
## Dependencies
None
## Example Playbook
```
- hosts: mariadb-slave1
  vars:
    mysql_packages:
      - mariadb
      - mariadb-server
      - MySQL-python
#  vars_files:
#    - vars/main.yml
  roles:
    -  role: ansible-role-mysql
