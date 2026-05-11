# Ansible Role: Node Exporter

## Description
This role installs and configures Prometheus Node Exporter as a systemd service.

## Features
- Installs Node Exporter
- Supports Debian and RedHat-based systems
- Runs as a systemd service
- Configurable via variables
- Idempotent

## Requirements
- Ansible 2.9+
- Linux (Debian/Ubuntu or RedHat-based)

## Role Variables

- node_exporter_version (default: 1.7.0) – Version of Node Exporter
- node_exporter_port (default: 9100) – Port used by Node Exporter
- node_exporter_user (default: node_exporter) – System user

## Example Playbook

- hosts: all
  become: yes
  roles:
    - node_exporter

## Test

Run locally:
ansible-playbook test.yml --become

## Dependencies
None

## License
MIT

## Author
endriu96
