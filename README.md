Assumptions:
1) passwordless ssh is enabled between Ansible host and client and ubuntu user is available on the client
2) Internet access is available for apt-get update
3) IP of the machine should be updated in the [all] tag in /etc/ansible/hosts #To check use: ansible-playbook testapp.yml


Implementation:
Execute command: ansible-playbook testapp.yml

