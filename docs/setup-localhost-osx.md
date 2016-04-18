# Setup localhost on OS X

This guide will show you how to setup localhost on OS X.

## 1. Requirements

- [OS X](http://www.ubuntu.com/desktop) >= **10.11**
- Logged in via SSH
- [Python](https://www.python.org) (should be preinstalled)
- [pip](https://pypi.python.org/pypi/pip) (`sudo easy_install pip`)
- [Xcode](https://developer.apple.com/xcode/) (do `xcode-select --install` and get [Xcode.app](https://itunes.apple.com/us/app/xcode/id497799835))
- [Homebrew](http://brew.sh) (`/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`)

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

Manual tasks which cannot be completed by Ansible are listed at [inventory/host_vars/localhost/manual.md](https://github.com/davisonio/localhost-devops/blob/master/inventory/host_vars/localhost/manual.md).
