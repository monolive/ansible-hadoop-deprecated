ansible-hadoop
==============

Ansible Playbook to install HDP. It should work on RHEL6, OEL6 and CentOS6. It has been tested on CentOS6

1- Edit hosts file to define cluster

2- Edit site.yml to select which service you would like to install by adding / removing services

3- Edit groups_var/all to adjust to your settings

Everything should be installed, but services won't be started. You will need to connect to ambari webui on port 8080 to start services manually

TODO : make the service start following the installation
