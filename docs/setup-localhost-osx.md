# Setup localhost on OS X

This guide will show you how to setup localhost on OS X.

## 1. Requirements

- [OS X](http://www.ubuntu.com/desktop) >= **10.11**
- Logged in via SSH
- [Python](https://www.python.org) + [pip](https://pypi.python.org/pypi/pip)
- [Git](https://git-scm.com)

## 2. Get Ansible

```
$ sudo pip install ansible
```

## 3. Get localhost DevOps

```
$ git clone https://github.com/davisonio/localhost-devops
$ cd localhost-devops
```

## 4. Run main.yml

Run the main playbook and hopefully everything should be working:

```
$ ansible-playbook main.yml
```

## 5. Complete manual tasks

Manual tasks which cannot be completed by Ansible are listed at [inventory/host_vars/localhost/manual.md].
