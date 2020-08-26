# ubuntu-autoinstall

An Ansible Playbook that performs an unattended Ubuntu Server 20.04.1 VM installation.

## Usage

Modify the values of the variables in **util_DeployUbuntu.yml** so they match your environment.

* sudo apt install python3 python3-pip xorriso
* pip3 install ansible pyvim pyvmomi
* git clone https://github.com/rutgerblom/ubuntu-autoinstall.git
* sudo ansible-playbook util_DeployUbuntu.yml
