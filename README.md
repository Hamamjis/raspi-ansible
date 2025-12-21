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


### Usage
```sh
ansible-playbook main.yml
```
