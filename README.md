# ubuntu-autoinstall

An Ansible Playbook that performs unattended Ubuntu Server 20.04 VM installations on VMware vSphere.

## Prerequisites

Prepare an Ubuntu machine by running the following commands:

* sudo apt update && sudo apt install python3 python3-pip git xorriso
* git clone https://github.com/rutgerblom/ubuntu-autoinstall.git ~/git/ubuntu-autoinstall
* pip3 install --upgrade -r ~/git/ubuntu-autoinstall/pip_requirements.txt
* ansible-galaxy collection install --upgrade -r ~/git/ubuntu-autoinstall/requirements.yml

## Usage

Modify the variables in ```Variables.yml``` so that they match your environment and your requirements. Start the Ubuntu Server deployment by running: ```ansible-playbook DeployUbuntu.yml```
