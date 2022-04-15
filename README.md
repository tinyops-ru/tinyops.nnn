# Ansible role for nnn

Tiny ansible role for [nnn](https://github.com/jarun/nnn).

## Getting started

Define variables for your groups\hosts:

```yaml

nnn_users: []

# Bookmarks
nnn_bms: 'r:/root'

# Plugins
nnn_plug: ''

nnn_profile_config_file: .bashrc

nnn_install_for_root: False
```

Minimal playbook:

```yaml
- hosts: web
  roles:
  - tinyops.nnn
```

### Use as git submodule

Add to your git:

```bash
git submodule add https://github.com/tinyops-ru/tinyops.nnn.git roles/tinyops.nnn
```

Init:

```bash
git submodule update --init --recursive --remote
```

## How it works

Role use os package manager for install package `nnn`.

Then adds to `.bash_profile` or `.bashrc` configuration.

### CentOS 6

Role will install static binary from role `files` dir.

## TODO

- Support `NNN_PLUG` override for each user
- Support plugins installation
