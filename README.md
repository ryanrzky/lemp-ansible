#### Install LEMP Stack Ubuntu

Cara install LEMP Stack (Linux, Nginx, MySQL, Php)


#### Edit Variable di `vars/vars.yaml`

Edit sesuai dengan kebutuhan

`php_version` untuk merubah versi php

`mysql_root_password` untuk password root mysql

`http_host` untuk domain atau IP

### Edit Host yang akan di remote di `hosts.yaml`

`ansible_user` user server target

`ansible_ssh_pass` password user target 

`192.168.99.11` ganti dengan IP server target

### Jalankan Ansible

```
ansible-playbook -i hosts.yaml main.yaml
```