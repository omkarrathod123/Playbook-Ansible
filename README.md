# Playbook-Ansible

## Ansible
Ansible is an open-source IT automation engine that automates provisioning, configuration management, application deplyment, orchestration tool.Ansible follow a push based Configration Management.

### Components of Ansible

1. Playbook: Ansible used YAML file to give instraction in Declarative configuration.
2. Inventory: Collaction of servers.Inventory file can have groups, An entry can be duplicate in many groups.

## Ansible Roles
Role is the primary mechanism for braking a playbook into multiple files.Roles are good for organizing task and encapsulating data needed and accomplish those task.

- **Default:** It stores the data about application.
- **File:** It containes files made to transferred to the remote virtual machine.
- **Handler:** Thay are triggers or task we can segregate all handlers required in playbook.
- **Meta:** This directory content files that establish rolls dependencies.
- **Task:** It containes all the task that is normally in the playbook.
- **Vars:**  Variables for the role can be specified in this directory and used in your configuration files both wars and Default stores variables.

## Installation on Ubuntu Server
1. Get and install update
```sh
sudo apt --purge autoremove
sudo apt update
sudo apt upgrade
```
2. Install software-properties-common
```sh
sudo apt -y install software-properties-common
```
3. Add ansible repository
```sh
sudo apt-add-repository ppa:ansible/ansible
```
4. Install Ansible
```sh
sudo apt install ansible
```
note:- Python 3 is required for ansible.
---