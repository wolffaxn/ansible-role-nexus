# Ansible Role - Sonatype Nexus

[![MIT licensed](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![GitHub last commit (branch)](https://img.shields.io/github/last-commit/wolffaxn/ansible-role-nexus/master.svg)](https://github.com/wolffaxn/ansible-role-nexus)

**Table of Contents**

<!-- toc -->

- [About](#about)
- [Requirements](#requirements)
- [Role Variables](#role-variables)
- [Dependencies](#dependencies)
- [Example Playbook](#example-playbook)
- [License](#license)

<!-- tocstop -->

## About

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

This project is licensed under the terms of the [MIT license](LICENSE).
