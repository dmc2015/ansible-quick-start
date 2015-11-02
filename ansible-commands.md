ansible -m ping -u vagrant all
# tell ansible to use the module (-m) ping and the user (-u) vagrant on all machines
# running a ping test on all machines




ansible-playbook basic-laybook-1.yaml -e "uservar=vagrant"
# tells ansible to run a playbook and to use the vagrant user when accessing the
# host for ssh access and installation


#NOTE
#Ansible will not make any changes that it does not need
#to. If packages and libraries are already installed
#ansible will not reinstall them but will return with a 'ok' response to let you know everything is okay.
