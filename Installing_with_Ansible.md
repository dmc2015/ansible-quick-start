Package Management with Ansible

- name: install httpd
  yum: name=httpd state=present


- name: install httpd
  apt: name=httpd state=present


Install a Set of packages

- name: install a set of packages
  yum: name={{ item }} state=present
  with_items:
    - httpd
    - php
    - git
    - mysql-client
