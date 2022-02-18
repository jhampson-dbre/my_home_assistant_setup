```bash
# install required roles and collections
ansible-galaxy role install -r requirements.yml -f
ansible-galaxy collection install -r requirements.yml -f

# bootstrap python3
ansible-playbook ./bootstrap_python.yml -i ./inventories/hosts -vv

# Install Home Assistant Supervised
ansible-playbook ./h_a_supervised_full_setup.yml -i ./inventories/hosts -vv
```