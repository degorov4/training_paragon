# training_paragon
Playbook and related artifacts for deploying Nginx in container via Ansible

# Prepare

### Ansible

First of all, you need Ansible.

I recommend you install Ansible via `pip`. Please refer to [documentation](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html#latest-releases-via-pip). In that case you will have a freedom to choose of installed version, because from time to time in ansible something breaks down.

### Docker

To run this playbook you need installed Docker on localhost machine. Please refer to [documentation](https://docs.docker.com/install/).

### Required sources

This project contains ansible-galaxy Nginx role and Ubuntu image for fast start. Please execute following command for preparing Ansbile run:

```bash
ansible-galaxy install --roles-path /etc/ansible/roles geerlingguy.nginx
```
# Ok, lets try

Execute following shell command for run playbook.yaml:

```bash
sudo ansible-playbook playbook.yaml
```
You can open http://localhost:80 in your browser and see Nginx welcome page. 

