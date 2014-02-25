#!/bin/bash

# Define Ganglia service
/usr/bin/curl -u admin:admin -H "X-Requested-By: ambari" -X POST http://{{ hostvars[groups['ambari_server'][0]]['ansible_fqdn'] }}:8080/api/v1/clusters/{{ hdp['CLUSTERNAME']}}/services/GANGLIA

# Define ganglia server
/usr/bin/curl -u admin:admin -H "X-Requested-By: ambari" -X POST http://{{ hostvars[groups['ambari_server'][0]]['ansible_fqdn'] }}:8080/api/v1/clusters/{{ hdp['CLUSTERNAME']}}/services/GANGLIA/components/GANGLIA_SERVER
/usr/bin/curl -u admin:admin -H "X-Requested-By: ambari" -X POST http://{{ hostvars[groups['ambari_server'][0]]['ansible_fqdn'] }}:8080/api/v1/clusters/{{ hdp['CLUSTERNAME']}}/hosts/{{ hostvars[groups['ambari_server'][0]]['ansible_fqdn'] }}/host_components/GANGLIA_SERVER

# Define server to monitor
/usr/bin/curl -u admin:admin -H "X-Requested-By: ambari" -X POST http://{{ hostvars[groups['ambari_server'][0]]['ansible_fqdn'] }}:8080/api/v1/clusters/{{ hdp['CLUSTERNAME']}}/services/GANGLIA/components/GANGLIA_MONITOR
{% for host in groups['datanode'] %}
/usr/bin/curl -u admin:admin -H "X-Requested-By: ambari" -X POST http://{{ hostvars[groups['ambari_server'][0]]['ansible_fqdn'] }}:8080/api/v1/clusters/{{ hdp['CLUSTERNAME']}}/hosts/{{ hostvars[host]['ansible_fqdn'] }}/host_components/GANGLIA_MONITOR
{% endfor %}

# Start the installation
/usr/bin/curl -u admin:admin -H "X-Requested-By: ambari" -X PUT -d '{"RequestInfo":{"context":"Install GANGLIA"}, "Body":{"ServiceInfo": {"state":"INSTALLED"}}}' http://{{ hostvars[groups['ambari_server'][0]]['ansible_fqdn'] }}:8080/api/v1/clusters/{{ hdp['CLUSTERNAME']}}/services/GANGLIA
