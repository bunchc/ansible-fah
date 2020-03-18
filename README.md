# ansible-fah

An Ansible role to install and configure the Folding-At-Home client.

## Example playbook

```yaml
- name: Install Folding At Home
  vars:
    fah_team: "52737"
    fah_user: "cody_bunch"
  hosts: folding_hosts
  roles:
    - ansible-fah
```

## Configuration

The FAH client can be configured rather extensively, at this time only a basic configuration is provided (user name, team, enable cpu/gpu).

## Summary

This role downloads and installs the 7.4.4 version of the [Folding @ Home](https://foldingathome.org/) client. It creates and applies a minimal configuration including running the web interface on port 7396. Finally it sets up a systemd service to manage it all.
