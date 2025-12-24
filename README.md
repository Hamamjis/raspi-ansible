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

The setup the machine, run the following command:
```sh
ansible-playbook playbooks/setup/main.yml
```

**Note:** If the users specified in `vars.yaml` don't exist, this will create them with the default password specified.

To change a user's password, run the following command:
```sh
ansible-playbook playbooks/change_password/main.yml
```