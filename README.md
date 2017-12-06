### Ansible Dynamic Inventory

Ansible inventory from a json file served via github pages

### Set environment variables

The url of your inventory file and the path to the inventory.sh script

`export INVENTORY_URL=https://darren-rose.github.io/ansible-inventory/inventory.json`

`export ANSIBLE_HOSTS=/path-to/inventory.sh`

### List hosts in a group 

`ansible --list-hosts webservers`

### Ping hosts in a group 

`ansible -m ping databases`

### Execute playbook on a group 

`ansible-playbook -e "hosts=databases" hostname.yml`

### Execute playbook on multiple groups 

`ansible-playbook -e "hosts=databases,webservers" hostname.yml`

### Execute playbook on a single host 

`ansible-playbook -e "hosts=host6.example.com" hostname.yml`
