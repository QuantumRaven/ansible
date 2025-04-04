# Ansible

This repository hosts all of my ansible playbooks for my sandboxed environments and some projects on Digital Ocean.

## Getting Started

To download the HTTPS repo:

```bash
git clone https://github.com/QuantumRaven/ansible.git
```

### Installation on RHEL distros

```bash
$ sudo dnf install ansible
```

## Usage

Wayfire Tiling Window Manager setup

Install applications with sudo_user.yaml first

```bash
$ ansible-playbook -i inventory.ini fedora_fourty_one/wayfire/base_system_setup/sudo_user.yaml -K --limit=[group_name or device_name]
```

Configure user profile

```bash
$ ansible-playbook -i inventory.ini fedora_fourty_one/wayfire/base_system_setup/user_setup.yaml --limit=[group_name or device_name]
```

KDE setup

Coming in the next update...
