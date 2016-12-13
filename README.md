Assumptions:
1) passwordless ssh is enabled between Ansible host and client and ubuntu user is available on the client
2) Internet access is available for apt-get update


Implementation:
Execute command: ansible-playbook -i <ip_address>, testapp.yml


