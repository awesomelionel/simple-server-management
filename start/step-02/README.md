# Update Ubuntu task
Here we are going to run updates to ubuntu via apt

ansible-playbook start/step-02/update.yml -i start/step-02/hosts -l host0.example.org

-i targeted inventory file
-l limit to host name

This will install:
- git
- vim
