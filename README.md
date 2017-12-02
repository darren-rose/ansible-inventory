### Ansible Dynamic Inventory

Ansible inventory from a json file served via github pages

### Step 1

Set the following environment variable to url of the json file

```export INVENTORY_FILE_URL=https://darren-rose.github.io/ansible-inventory/inventory.json```

### Step2 

```ansible -i ./inventory.sh -m ping databases```