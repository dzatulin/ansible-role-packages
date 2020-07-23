# Ansible Packages Role
Role for installing, removing and updating packages
## Requirements
Ansible version: 2.9
## Dependencies
None
## Example Playbook
```
  - hosts: "{{ var }}"
     install_all_package_updates: true
     install_packages:
     - epel-release
     - mc
     - vim
   roles:
     - ansible-role-packages
   tasks:
     - name: set timezone to UA_Kiev
       timezone:
         name: Europe/Kiev

