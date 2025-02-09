# HW_1_Ansible

Deploy Nginx Web Server

Run the following command to install and configure Nginx on port 8080:
```shell
ansible-playbook -i hosts deploy_nginx.yml --key-file your_key.pem
```

After execution, visit:
http://your_server_ip:8080

Undeploy (Remove) Nginx

Run the following command to stop and uninstall Nginx:

```shell
ansible-playbook -i hosts undeploy_nginx.yml --key-file your_key.pem
```

Note:
Replace your_key.pem with the actual .pem key file for SSH access.
Replace your host name and keys in inventory file.
Ensure the .pem file has correct permissions:
```
chmod 400 your_key.pem 
```