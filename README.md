## Project structure

```
ansible-devops/
│── inventory/              # Inventory files (grouped by environment)
│   ├── dev.ini             # Development servers
│   ├── prod.ini            # Production servers
│── playbooks/              # Ansible playbooks
│   ├── setup-jenkins.yml   # Playbook to set up Jenkins
│   ├── setup-k8s.yml       # Playbook to configure Kubernetes nodes
│── roles/                  # Ansible roles for modular automation
│   ├── common/             # Common configurations (e.g., user setup)
│   ├── jenkins/            # Role for setting up Jenkins
│   ├── kubernetes/         # Role for Kubernetes setup
│── files/                  # Static files (configs, scripts, etc.)
│── templates/              # Jinja2 templates for dynamic configs
│── vars/                   # Variables for playbooks
│── group_vars/             # Group-wide variables
│── ansible.cfg             # Ansible configuration file
│── README.md               # Documentation

```

## deploy the configuration
`ansible-playbook playbooks/setup-docker-jenkins.yml`