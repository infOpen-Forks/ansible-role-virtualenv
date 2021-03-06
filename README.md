# virtualenv

[![Build Status](https://img.shields.io/travis/Temelio/ansible-role-virtualenv/master.svg?label=travis_master)](https://travis-ci.org/Temelio/ansible-role-virtualenv)
[![Build Status](https://img.shields.io/travis/Temelio/ansible-role-virtualenv/develop.svg?label=travis_develop)](https://travis-ci.org/Temelio/ansible-role-virtualenv)
[![Updates](https://pyup.io/repos/github/Temelio/ansible-role-virtualenv/shield.svg)](https://pyup.io/repos/github/Temelio/ansible-role-virtualenv/)
[![Python 3](https://pyup.io/repos/github/Temelio/ansible-role-virtualenv/python-3-shield.svg)](https://pyup.io/repos/github/Temelio/ansible-role-virtualenv/)
[![Ansible Role](https://img.shields.io/ansible/role/8592.svg)](https://galaxy.ansible.com/Temelio/virtualenv/)

Install virtualenv package.

## Requirements

This role requires Ansible 2.2 or higher,
and platform requirements are listed in the metadata file.

## Testing

This role use [Molecule](https://github.com/metacloud/molecule/) to run tests.

Local and Travis tests run tests on Docker by default.
See molecule documentation to use other backend.

Currently, tests are done on:
- Debian Jessie
- Ubuntu Trusty
- Ubuntu Xenial

and use:
- Ansible 2.2.x
- Ansible 2.3.x
- Ansible 2.4.x

### Running tests

#### Using Docker driver

```
$ tox
```

## Role Variables

### Default role variables

``` yaml
virtualenv_packages: "{{ _virtualenv_packages }}"
```

## Dependencies

None

## Example Playbook

``` yaml
- hosts: servers
  roles:
    - { role: Temelio.virtualenv }
```

## License

MIT

## Author Information

Alexandre Chaussier (for Temelio company)
- http://www.temelio.com
- alexandre.chaussier [at] temelio.com
