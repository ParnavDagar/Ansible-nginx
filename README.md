# Ansible Playbooks for NGINX Configuration and File Copy

This repository contains Ansible playbooks to perform two operations on a remote machine with an NGINX server:

1. Updating the NGINX configuration to listen on a different port and copying the updated file to remote remote machine.
2. Copying a local `index.nginx-debian.html` file to the remote machine's web directory.

## Description


- **Copy Local File to Remote Machine**:

  A playbook to copy a local `index.nginx-debian.html` file from `/var/www/html/` to the `/var/www/html/` directory on the remote machine.
  - You can provide any index.html file to make the changes.

  A playbook to copy the updated NGINX configuration file at `/etc/nginx/sites-enabled/default` to the remote machine at `/etc/nginx/sites-enabled/default`.

## Usage

1. Ensure Ansible is installed on your machine.
2. Update the `hosts` file with the hostname or IP address of your remote machine.
3. Run the following command to execute the playbooks:

```bash
ansible-playbook <PLAYBOOK FILE NAME> -i <HOST FILE NAME>
