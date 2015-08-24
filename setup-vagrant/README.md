Run this:

ansible-playbook -c paramiko -i setup-vagrant/hosts setup-vagrant/setup.yml --ask-pass --sudo

enter the ssh password _vagrant_

If there's any paramiko errors, please delete the ip 192.168.33.111 from the known hosts file
