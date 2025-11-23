# simple.haproxy

[![Maintainer](https://img.shields.io/badge/maintained%20by-Simple-Ansible-e00000?style=flat-square)](https://github.com/Simple-Ansible)
[![License](https://img.shields.io/github/license/Simple-Ansible/simple.haproxy?style=flat-square)](https://github.com/Simple-Ansible/simple.haproxy
/blob/main/LICENSE)
[![Release](https://img.shields.io/github/v/release/Simple-Ansible/simple.haproxy?style=flat-square)](https://github.com/Simple-Ansible/simple.hapro
xy/releases)
[![Status](https://img.shields.io/github/workflow/status/Simple-Ansible/simple.haproxy/Ansible%20Molecule?style=flat-square&label=tests)](https://gi
thub.com/Simple-Ansible/simple.haproxy/actions?query=workflow%3A%22Ansible+Molecule%22)
[![Ansible 
Galaxy](https://img.shields.io/badge/ansible-galaxy-black.svg?style=flat-square&logo=ansible)](https://galaxy.ansible.com/Simple-Ansible/haproxy)[![
Ansible version](https://img.shields.io/badge/ansible-%3E%3D2.10-black.svg?style=flat-square&logo=ansible)](https://github.com/ansible/ansible)

⭐ Star us on GitHub — it motivates us a lot!

Simple manage haproxy

**Platforms Supported**:

| Platform | Versions |
|----------|----------|
| Debian | trixie |

## ⚠ Requirements

Ansible >= 2.20.

### Ansible role dependencies

None.

## ⚡ Installation

### Install with Ansible Galaxy

```shell
ansible-galaxy install simple.haproxy
```

### Install with git

If you do not want a global installation, clone it into your `roles_path`.

```bash
git clone git@github.com:Simple-Ansible/simple.haproxy.git  simple.haproxy
```

But I often add it as a submodule in a given `playbook_dir` repository.

```bash
git submodule add git@github.com:Simple-Ansible/simple.haproxy.git roles/simple.haproxy
```

As the role is not managed by Ansible Galaxy, you do not have to specify the
github user account.

### ✏ Example Playbook

Basic usage is:

```yaml
- hosts: all
  roles:
    - role: simple.haproxy
  tags:
    - haproxy
```

## ⚙ Role Variables

Variables are divided in three types.

The **default vars** section shows you which variables you may
override in your ansible inventory. As a matter of fact, all variables should
be defined there for explicitness, ease of documentation as well as overall
role manageability.

The **context variables** are shown in section below hint you
on how runtime context may affects role execution.

### Default variables
Role default variables from `defaults/main.yml`.

| Variable Name | Value |
|---------------|-------|
| haproxy_official_repo | False |
| haproxy_version | 3.2 |
| haproxy_cfg_template |  |
| haproxy_errors_local_dir |  |
| haproxy_ssl_local_dir |  |

### Context variables

Those variables from `vars/*.{yml,json}` are loaded dynamically during task
runtime using the `include_vars` module.

Variables loaded from `vars/main.yml`.


## Author Information

:>)
