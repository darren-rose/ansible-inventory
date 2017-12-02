### Ansible Dynamic Inventory

Ansible inventory from a json file served via github pages

### Set environment variable

Set the following environment variable to url of your json file

e.g. `export INVENTORY_FILE_URL=https://darren-rose.github.io/ansible-inventory/inventory.json`

### List hosts in webservers group 

`ansible -i ./inventory.sh --list-hosts webservers`

### Ping databases group 

`ansible -i ./inventory.sh -m ping databases`

### Execute playbook on databases group 

`ansible-playbook -i ./inventory.sh  -e "hosts=databases" hostname.yml`

### Execute playbook on a single host 

`ansible-playbook -i ./inventory.sh  -e "hosts=host6.example.com" hostname.yml`
