ansible-galaxy role install -r requirements.yml -f
ansible-galaxy collection install -r requirements.yml -f
ansible-playbook ./h_a_supervised_full_setup.yml -i ./inventories/hosts -vv

--extra-vars "docker_apt_arch=arm64"