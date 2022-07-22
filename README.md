install ansible roles:  

- you can use ```make init``` command(need installed make)  

OR   

- ```ansible-galaxy role install -f -r requirements.yml --roles-path galaxy_roles```

they will be downloaded to ```galaxy_roles``` folder and .gitignored

 

run playbook: ```ansible-playbook  site.yml --diff -K``` and input sudo password


also specify your vars in ```inventory/prod.yml```




## example_vars:
```
ansible_connection: ssh ---   *connection method to host(default)*
ansible_user: udjin  ---   *remote user with sudo group*
ansible_ssh_private_key_file: /home/udjin/.ssh/id_ed25519 --- *ssh private key file path*``` 