# Ansible:

Main important thing that we need to ensure is our Ansible machine should be able to SSH to the machines mentioned in the inventory file

# Few Basics of Ansible: 
## Ansible: It is a CM tool and latest version is 7.0

As Ansible is a python tool installed python 3 and then installed ansible. 

sudo yum install python3-pip -y
sudo pip3 install pip --upgrade
sudo pip3 install ansible

## Inventory: This is a file which will provide ansible the DNS names or IP's. 
The Default group in this file is all. 

## Sample Ansible manual command:
ansible -i inv -e ansible_user=centos -e ansible_password=DevOps321 -m shell -a "df -h"

-i                    :    Inventory file
-e                    :    Extra argument
ansible_user          :    user name
ansible_password      :    password
-m                    :    module
-a                    :    argument

## Ansible user YAML langauge which is a presentation language

## YAML Basics:
Directory   :   A key value pair is called directory
List        :   A key with multiple values is called list
Map         :   A key with multiple key value pairs is called map. 

## Ansible pull needs ansible to be installed on the node.

