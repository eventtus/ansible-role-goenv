# Ansible Role for goenv

[![Build Status](https://travis-ci.org/eventtus/ansible-role-goenv.svg?branch=master)](https://travis-ci.org/eventtus/ansible-role-goenv)
[![GitHub issues](https://img.shields.io/github/issues/eventtus/ansible-role-goenv.svg?maxAge=2592000)](https://github.com/eventtus/ansible-role-goenv/issues)

An Ansible role that installs Goenv and Go on Ubuntu and Debian

## Requirements

None

## Role Variables

### Defaults

    goenv_user: "ubuntu"
    goenv_path: ".goenv"
    goenv_version: "0.0.5"
    goenv_versions:
    - 1.6.1

### Description

  - `goenv_user`: System user to install goenv for.
  - `goenv_path`: Install path.
  - `goenv_version`: Version of goenv to install.
  - `goenv_versions`: Array of versions of Go to install.

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
      - role: eventtus.goenv
        goenv_versions:
        - 1.6.1
        - 1.7.0

## License

MIT/BSD

## Credits

[![Eventtus](http://assets.eventtus.com/logos/eventtus/standard.png)](http://eventtus.com)

Created by [Omar Abdel-Wahab](https://github.com/owahab) and sponsored by [Eventtus](http://eventtus.com).
