Multi-Environment Deployment (Ansible)
- playbook: playbooks/deploy.yml
- inventories: inventories/{dev,stage,prod}
- role: roles/webserver
Run (example): ansible-playbook -i inventories/dev playbooks/deploy.yml
