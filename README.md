# ubuntu-autoinstall

An Ansible Playbook that performs an unattended Ubuntu Server 20.04.1 VM installation.

## Prerequisites

Prepare an Ubuntu machine by running the following commands:

* sudo apt install python3 python3-pip git xorriso
* sudo pip3 install ansible pyvim pyvmomi
* git clone https://github.com/rutgerblom/ubuntu-autoinstall.git
* cd ubuntu-autoinstall

## Usage

Modify the variables in **util_DeployUbuntu.yml** so that they match your environment. Start the Ubuntu Server deployment by running:
<br>
**sudo ansible-playbook DeployUbuntu.yml**
