# Ansible Role: Spruce

[![CI](https://github.com/rholmboe/ansible-role-spruce/actions/workflows/ci.yml/badge.svg)](https://github.com/rholmboe/ansible-role-spruce/actions/workflows/ci.yml)
[![Ansible Role](https://img.shields.io/ansible/role/57227?logo=ansible)](https://galaxy.ansible.com/rholmboe/spruce)
[![Ansible Quality Score](https://img.shields.io/ansible/quality/57227?logo=ansible)](https://galaxy.ansible.com/rholmboe/spruce)

Installs [Spruce](https://github.com/geofffranks/spruce), a Go-based BOSH template merge tool.

An honest duplication of [ansible-role-packer](https://github.com/geerlingguy/ansible-role-packer/) by [Jeff Geerling](https://www.jeffgeerling.com/)

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```
    spruce_version: "1.29.0"
```

The spruce version to install.

```
    spruce_arch: "amd64"
```

The system architecture (e.g. `386` or `amd64`) to use.

```
    spruce_bin_path: /usr/local/bin
```

The location where the spruce binary will be installed (should be in system `$PATH`).

The user/group which should own binary.

```
    spruce_user: "root"
    spruce_group: "root"
```

## Dependencies

None.

## Example Playbook

    - hosts: servers
      roles:
        - rholmboe.spruce

## License

MIT / BSD

## Author Information

This role was created in 2021 by [Richard Holmboe](https://about.me/rholmboe)
