Roles - A tool that allows you to create reusable building blocks or pieces, components are intended to be reusable and swapped. They are intended to make things easy in complex situations.


Project organization tool
Resuable components
Defined filesystem structure
Show: parametererized roles

Playbook File Structure

webserver/
  files
    epel.repo.j2
    rpm-gpg-key
  Handlers
    main.yml
  tasks
    main.yml
  Templates
    httpd.conf.j2

Roles can have the following
  variables
  defaults
  dependencies


http://galaxy.ansible.com - collection of ansible roles
