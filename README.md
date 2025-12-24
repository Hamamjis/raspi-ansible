# Raspberry Pi Ansible

### Requirements

- The target user must have sudo privileges

### Setup

- Copy `inventory.sample.yml` to `inventory.yml` and set the values accordingly
- Copy `vars.sample.yml` to `vars.yml` and set the values accordingly
- Install dependencies:
```sh
ansible-galaxy role install -r requirements.yml
```
- Ensure `passlib` is installed. On Fedora, it can be installed by running the following command:
```sh
sudo dnf install python3-passlib
```

### Usage

```sh
ansible-playbook playbooks/setup/main.yml
```
