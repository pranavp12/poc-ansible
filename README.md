Assumptions:
1) passwordless ssh is enabled between Ansible host and client and ubuntu user is available on the client
2) This playbook is tested on ubuntu 14.04

To enable passwordless ssh:
ssh-keygen
ssh-copy-id user@host
ssh user@host

Implementation:
Enter IP Address of the host in hosts file under hosts tag
Execute command: ansible-playbook testapp.yml --extra-vars "hosts=<ip-address>"

Known issues: 
Tomcat does not start on 2nd instance i.e port 8181 from playbook. It has to be started manually.
Please start it using: sudo /usr/share/tomcat7/bin/startup.sh and sudo /usr/share/tomcat7-instance2/bin/startup.sh
HAProxy playbook is not tested


