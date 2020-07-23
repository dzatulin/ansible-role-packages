Ansible Packages Role

## Example Playbook
  
 - hosts: "{{ var }}"
   vars:
     install_all_package_updates: true
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
   roles:
     - ansible-role-packages
   tasks:
     - name: set timezone to UA_Kiev
       timezone:
         name: Europe/Kiev
