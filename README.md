Aible Role Packages

- name: update
  hosts: "{{ var }}"
  vars:
    swap_file_size_mb: '2048'
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
    - ansible-packages
    - geerlingguy.swap
    - geerlingguy.git
    - do-agent
  tasks:
    - name: set timezone to UA_Kiev
      timezone:
        name: Europe/Kiev
