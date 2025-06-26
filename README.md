# Configuration management with Ansible.
The Utility installs basic packeges and nginx(webserver).
Then the role app will deploy application for the webserver.

## Peoject url: https://roadmap.sh/projects/configuration-management

## Steps to follow:
1. Please update inventory.ini has the right server IP, user, and SSH key path.
2. Make sure setup.yml has your actual public key content for ssh_public_key.
'''

# Run your playbook:
** ansible-playbook -i inventory.ini setup.yml

# Run only the app role
** ansible-playbook setup.yml --tags "app"
