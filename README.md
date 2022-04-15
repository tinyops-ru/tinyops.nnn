# Ansible role for nnn

Tiny ansible role for [nnn](https://github.com/jarun/nnn).

## Getting started

```yaml

nnn_users: []

# Bookmarks
nnn_bms: 'r:/root'

# Plugins
nnn_plug: ''

nnn_profile_config_file: .bashrc

nnn_install_for_root: False
```

## CentOS 6

Install static binary from role `files` dir.

## TODO

- Support `NNN_PLUG` override for each user
- Support plugins installation
