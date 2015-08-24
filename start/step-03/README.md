# Installing NGINX

In this step, we install and nginx 'role' via Ansible Galaxy;

$ ansible-galaxy install jdauphant.nginx
$ ansible-galaxy install geerlingguy.ruby

This will install the role into /etc/ansible/roles/jdauphant.nginx
and /etc/ansible/roles/geerlingguy.ruby

Then we attach it to the site.yml file.

- hosts: web
  roles:
    - role: jdauphant.nginx
    - role: geerlingguy.ruby

Run the command 

$ ansible-playbook start/step-03/site.yml -i start/step-03/hosts

BOOM NGINX + RUBY
