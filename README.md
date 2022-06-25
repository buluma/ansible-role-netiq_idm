# [netiq-idm](#netiq-idm)

Installs NetIQ Identity Manager

|GitHub|GitLab|Quality|Downloads|Version|Issues|Pull Requests|
|------|------|-------|---------|-------|------|-------------|
|[![github](https://github.com/buluma/ansible-role-netiq-idm/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/ansible-role-netiq-idm/actions)|[![gitlab](https://gitlab.com/buluma/ansible-role-netiq-idm/badges/master/pipeline.svg)](https://gitlab.com/buluma/ansible-role-netiq-idm)|[![quality](https://img.shields.io/ansible/quality/)](https://galaxy.ansible.com/buluma/netiq-idm)|[![downloads](https://img.shields.io/ansible/role/d/)](https://galaxy.ansible.com/buluma/netiq-idm)|[![Version](https://img.shields.io/github/release/buluma/ansible-role-netiq-idm.svg)](https://github.com/buluma/ansible-role-netiq-idm/releases/)|[![Issues](https://img.shields.io/github/issues/buluma/ansible-role-netiq-idm.svg)](https://github.com/buluma/ansible-role-netiq-idm/issues/)|[![PullRequests](https://img.shields.io/github/issues-pr-closed-raw/buluma/ansible-role-netiq-idm.svg)](https://github.com/buluma/ansible-role-netiq-idm/pulls/)|

## [Example Playbook](#example-playbook)

This example is taken from `molecule/default/converge.yml` and is tested on each push, pull request and release.
```yaml
---
- name: converge
  hosts: all
  become: yes
  gather_facts: yes

  roles:
    - role: buluma.netiq_idm
```

The machine needs to be prepared. In CI this is done using `molecule/default/prepare.yml`:
```yaml
---
- name: prepare
  hosts: all
  become: yes
  gather_facts: no

  roles:
    - role: buluma.bootstrap
```


## [Role Variables](#role-variables)

The default values for the variables are set in `defaults/main.yml`:
```yaml
---
# defaults file for netiq-idm
SERVER_KEYSTORE: /etc/ssl/servercerts/server.p12
```

## [Requirements](#requirements)

- pip packages listed in [requirements.txt](https://github.com/buluma/ansible-role-netiq-idm/blob/main/requirements.txt).


## [Context](#context)

This role is a part of many compatible roles. Have a look at [the documentation of these roles](https://buluma.github.io/) for further information.

Here is an overview of related roles:

![dependencies](https://raw.githubusercontent.com/buluma/ansible-role-netiq-idm/png/requirements.png "Dependencies")

## [Compatibility](#compatibility)

This role has been tested on these [container images](https://hub.docker.com/u/buluma):

|container|tags|
|---------|----|
|el|all|
|fedora|all|
|debian|all|
|ubuntu|all|

The minimum version of Ansible required is 2.4, tests have been done to:

- The previous version.
- The current version.
- The development version.



If you find issues, please register them in [GitHub](https://github.com/buluma/ansible-role-netiq-idm/issues)

## [Changelog](#changelog)

[Role History](https://github.com/buluma/ansible-role-netiq-idm/blob/master/CHANGELOG.md)

## [License](#license)

Apache-2.0

## [Author Information](#author-information)

[Michael Buluma](https://buluma.github.io/)
