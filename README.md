You can use 'make init'(need instal make) to install roles or "ansible-galaxy role install -f -r requirements.yml --roles-path galaxy_roles"

to run playbook: 'ansible-playbook  site.yml --diff '

also specify vars in inventory/prod.yml

example:

ansible_connection: ssh
ansible_user: udjin
ansible_ssh_private_key_file: /home/udjin/.ssh/id_ed25519

