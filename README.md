# ubuntu-autoinstall

An Ansible Playbook that performs an unattended Ubuntu Server 20.04.2 VM installation on vSphere.

## Prerequisites

Prepare an Ubuntu machine by running the following commands:

* sudo apt update && sudo apt install python3 python3-pip git xorriso
* git clone https://github.com/rutgerblom/ubuntu-autoinstall.git ~/git/ubuntu-autoinstall
* pip3 install --upgrade -r ~/ubuntu-autoinstall/pip_requirements.txt
* ansible-galaxy collection install --upgrade -r ~/ubuntu-autoinstall/requirements.yml

## Usage

Modify the variables in **DeployUbuntu.yml** so that they match your environment. Start the Ubuntu Server deployment by running:
<br>
**ansible-playbook DeployUbuntu.yml**
