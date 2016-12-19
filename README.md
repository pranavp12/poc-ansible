Assumptions:
1) passwordless ssh is enabled between Ansible host and client and ubuntu user is available on the client
2) Internet access is available for apt-get update


Implementation:
Execute command: ansible-playbook testapp.yml --extra-vars "target=<ip-address>"

PS: If implementation stops in the step to install java, please run: sudo apt-get -f install on the host and re-run the playbook
