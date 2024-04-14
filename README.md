# Ansible role apache

![GitHub](https://img.shields.io/github/license/jomrr/ansible-role-apache) ![GitHub last commit](https://img.shields.io/github/last-commit/jomrr/ansible-role-apache) ![GitHub issues](https://img.shields.io/github/issues-raw/jomrr/ansible-role-apache)

**Ansible role for setting up apache httpd.**

## Description

Install apache httpd from os repositories and configure
  - default server
  - modules
  - reverse proxy
  - TLS
  - virtual hosts
for version 2.4 or greater. The role will not work with version 2.2.

## Prerequisites

This role has no special prerequisites.

### System packages (Fedora)

- `python3` (Python 3.8 or later)
- `httpd (>= 2.4)`

### Python (requirements.txt)

- ansible >= 2.15

## Dependencies (requirements.yml)

This role has no dependencies.

## Supported Platforms

| OS Family | Distribution | Version | Container Image |
|-----------|--------------|---------|-----------------|
| RedHat | AlmaLinux | latest | [jomrr/molecule-almalinux:latest]( https://hub.docker.com/r/jomrr/molecule-almalinux ) |
| Alpine | Alpine | latest | [jomrr/molecule-alpine:latest]( https://hub.docker.com/r/jomrr/molecule-alpine ) |
| Archlinux | Archlinux | latest | [jomrr/molecule-archlinux:latest]( https://hub.docker.com/r/jomrr/molecule-archlinux ) |
| Debian | Debian | latest | [jomrr/molecule-debian:latest]( https://hub.docker.com/r/jomrr/molecule-debian ) |
| RedHat | Fedora | latest | [jomrr/molecule-fedora:latest]( https://hub.docker.com/r/jomrr/molecule-fedora ) |
| Suse | OpenSuse Leap | latest | [jomrr/molecule-opensuse-leap:latest]( https://hub.docker.com/r/jomrr/molecule-opensuse-leap ) |
| Suse | OpenSuse Tumbleweed | latest | [jomrr/molecule-opensuse-tumbleweed:latest]( https://hub.docker.com/r/jomrr/molecule-opensuse-tumbleweed ) |
| Debian | Ubuntu | latest | [jomrr/molecule-ubuntu:latest]( https://hub.docker.com/r/jomrr/molecule-ubuntu ) |

## Role Variables

No role default variables specified, see [defaults/main.yml](defaults/main.yml).

## Example Playbook

Example playbooks(s) that show how to use this role.

## Simple example playbook

A simple default example playbook for using jomrr.apache.
```yaml
---
# name: "jomrr.apache"
# file: "playbook_apache.yml"

- name: "PLAYBOOK | apache"
  hosts: "apache_hosts"
  gather_facts: true
  roles:
    - role: "jomrr.apache"
```

## Author(s) and License

- :octocat:                 Author::    [jomrr](https://github.com/jomrr)
- :triangular_flag_on_post: Copyright:: 2024, Jonas Mauer
- :page_with_curl:          License::   [MIT](LICENSE)

## References

- [Apache HTTP Server Documentation](https://httpd.apache.org/docs/)
- [ArchWiki - Apache HTTP Server](https://wiki.archlinux.org/title/Apache_HTTP_Server)
- [Fedora Quick Docs - Getting started with Apache HTTP Server](https://docs.fedoraproject.org/en-US/quick-docs/getting-started-with-apache-http-server/)

---
