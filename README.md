ansible-hadoop
==============

Ansible Playbook to install HDP. It should work on RHEL6, OEL6 and CentOS6. It has been tested on CentOS6

1- Edit hosts file to define cluster

2- Edit site.yml to select which service you would like to install by adding / removing services

3- Edit variable files in vars folder. 

The following files are mandatory
 - network_info
 - repository_info

The following files are optionals
 - users

Everything should be installed, but services won't be started. You will need to connect to ambari webui on port 8080 to start services manually

NB :
Following the installation, you can find all scripts + logfiles in /root/ambari-install

Hive server will also run 
 - metastore
 - mysql server
 - webhcat
 - hcatalog

Ambari Server will run 
 - ganglia
 - nagios

TODO : make the service start following the installation
