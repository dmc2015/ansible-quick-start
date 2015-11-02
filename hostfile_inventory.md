EXAMPLE 1
[web]
webserver-1.example.com
webserver-2.example.com


[db]
dbserver-1.example.com


EXAMPLE 2

[web]
web-server[01:25].example.com
#specifies a range of characters
#that are in this list (1 through 25)

[db]
dbserver-[a:f].example.com
#specifies a range of characters
#that are in this list (a through f)

Example 3 - set variables and overide addresses

Non-standard SSH ports:

webserver.example.com:2222

SSH Tunnel:
  myhost ansible_ssh_port=5555
    ansible_ssh_host=192.168.0.1






#NOTES
#A list of host but it will be organized into groups of hosts

#This file can come from several places
# A flat file, directory of files or
#a cloud provisioning envrionment;
#EC2, Rackspace, Google Compute Engine, etc.
