## Ansible Role For Substrate Node

This role checks the substrates binary URL and if the URL contains `.zip` or `.tar.gz`, it download and unzip a
the substrate binary on a specific path else it just download the substrate binary on a target location.

## Requirements

- Ansible >= 2.7

## Environment Variables

All variables are stored in `vars/main.yml` and can be overidden

## Playbook

Use it in a playbook as follows:

```
- hosts: all
  connection: local
  roles:
    - download_substrate_binary
```
