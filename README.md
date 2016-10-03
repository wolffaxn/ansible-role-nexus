# Ansible Role - Sonatype Nexus

[![MIT licensed](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/wolffaxn/ansible-role-nexus/master/LICENSE)

Installs Sonatype Nexus (OSS) for RedHat/CentOS linux servers.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values:

    nexus_version: 2.13.0-01

    nexus_download_path: /tmp
    nexus_download_cleanup: true
    nexus_install_path: /usr/local
    nexus_run_path: /var/run/nexus
    nexus_working_path: /var/nexus

    nexus_user: nexus
    nexus_group: nexus
    nexus_user_shell: /bin/bash

    nexus_port: 8081

## Dependencies

None.

## Example Playbook

For RHEL / CentOS

```yaml
---
  - hosts: localhost
    become: true
    become_method: sudo
    remote_user: root
    roles:
      - ansible-role-nexus
```
## License

Licensed under the MIT License. See the [LICENSE file](LICENSE) for details.

## Author Information

This role was created by Alexander Wolff.
