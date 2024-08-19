# Steps to a working SFTP server replacement for mft
## Setup
* Populate the users yaml file
* Note the dataglide user is a special case that can access and delete all files

## In Azure
* Create a new Resource Group
* Create a Public IP 
* Create a disk (100GB should be enough)
* Create an ubuntu 24.04 VM
* Assign the public IP to the VM
* Allow connections on port 2222

## On the VM
* Mount the disk to /mnt/sftp
* Install Ansible
* Run the main.yaml playbook
