Deployment of Web Servers on Cloud

This is a simple project to Automate Deployment of Apache Web Servers on Multiple hosts / on AWS. 

Pre-requisites :
1. Creation of 2 eC2 Instances on AWS with public IP Addresses and access to SSH port 22 and http port 80 enabled.
2. Access key downloaded and stored on local for SSH connection.
3. SSH connection established to both ec2 instances from remote machine.
4. Ansible installed and configured on remote machine.

Steps:

1. Update the host.yml which is the inventory file with Public IP Address of ec2 instances obtained from AWS console.

2. Run the Ansible playbook using below command,

   " Ansible-playbook -i hosts.yml apacheinstall.yml

3. Playbook installs Apache webservers on both the instances simultaneously.

4. Verify by entering IP address of each machine on web browser.
