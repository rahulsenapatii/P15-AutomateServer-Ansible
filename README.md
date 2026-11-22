# Project 15: Automate Server Config with Ansible

Remote configuration automation using an Ansible controller to provision and configure an Nginx web server on an AWS EC2 instance (`ap-south-1`) over custom SSH port `2222`.

## Files
- `ansible.cfg`: Controller defaults (inventory path, host key checking disabled)
- `inventory.example.ini`: Inventory template for managed web server nodes on port `2222`
- `webserver.yml`: Playbook to install Nginx, enable the service, and deploy custom `index.html`

## Usage
`ansible webservers -m ping`
`ansible-playbook webserver.yml`
