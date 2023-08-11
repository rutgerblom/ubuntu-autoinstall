# ubuntu-autoinstall

An Ansible Playbook that performs unattended Ubuntu Server 22.04 VM installations on VMware vSphere.

## Prerequisites

Prepare an Ubuntu machine as Ansible Controller by running the following commands:

* ```sudo apt update && sudo apt install python3 python3-pip git p7zip-full xorriso```
* ```git clone https://github.com/rutgerblom/ubuntu-autoinstall.git ~/git/ubuntu-autoinstall```
* ```pip3 install --upgrade -r ~/git/ubuntu-autoinstall/pip_requirements.txt```
* ```ansible-galaxy collection install --upgrade -r ~/git/ubuntu-autoinstall/requirements.yml```

## Usage

Copy the ```variables_sample.yml``` file to ```variables.yml``` and modify the settings so that they match your environment and your requirements. Start the Ubuntu Server deployment by running: ```ansible-playbook DeployUbuntu.yml```
