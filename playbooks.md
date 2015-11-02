Playbooks

Playbooks contain tasks
  Tasks contain Modules

  Everything is sequentially ordered-strict dependency ordering. Handlers can be triggered by tasks and will run at the end once.

  ## Happens in order, top-bottom
  ## Except a handler it will run at the end and it only runs once even if it is called multiple times in a playbook. It will not run if it is not needed.

  Tasks - Tasks call a module and may have parameters with it. You are capable of writing your own modules.


Example of a Task
  tasks:
  - name: ensure apache is at the latest version
    yum: name=httpd state=latest

  -name: write the apache config file
   template: src=tempaltes/httpd.j2 dest=/etc/httpd.config

   - name: ensure apache is running
     service: name=httpd state=started
