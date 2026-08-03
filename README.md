ANSIBLE-IAC-ROLE-FIREWALLD
==========================
**COPYRIGHT** 2026 Arsi Atomi  
**LICENSE** MIT License [LICENSE](LICENSE)  
**AUTHORS**  
- Arsi Atomi <arsi@atomi.sh>

Overview
--------

This ansible role is meant for easier firewalld management specially with ipsets.

This role uses only ansible.builtin.* ansible modules and firewall-cmd command.

Requirements
------------

Control machine:
- Ansible version 2.11 or later

Target machine:
- DNF package manager

Repository checkout
-------------------

This role includes the shared task library as a Git submodule under
`tasks/shared`.

Clone the repository with submodules:

```bash
git clone --recurse-submodules https://github.com/idarsi/ansible-iac-role-firewalld.git
```

If you already cloned the repository without submodules, initialize them with:

```bash
git submodule update --init --recursive
```

Operations
----------

Operation                       | State               |
--------------------------------|---------------------|
Installing Firewalld            | present             |
Starting Firewalld service      | started             |
Stopping Firewalld service      | stopped             |


Code Quality
------------

This project adheres to the [Ansible Lint](https://ansible-lint.readthedocs.io) **production** profile, ensuring high-quality and production-ready configuration management.
