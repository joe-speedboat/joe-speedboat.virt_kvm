# Ansible Role: joe-speedboat.virt_kvm

An Ansible Role to install and configure a kvm host on hetzner machine.

## Motivation

[KVM](https://www.linux-kvm.org/page/Main_Page) in combination with
[libvirt](https://libvirt.org/) is the major Linux hypervisor. Installing and
configuring KVM is a very common task for most operators and engineers.

## Description

This role configures a KVM hypervisor:

-   install qemu-kvm
-   install libvirt
-   install [ksm](https://www.linux-kvm.org/page/KSM) support and service
-   install [kvm nesting](https://www.linux-kvm.org/page/Nested_Guests) support
-   install some kvm/virsh tools: https://github.com/joe-speedboat/shell.scripts
-   install OPNsense Firewall
-   install CentOS VM from Cloud Image

## Installation

Install from [Ansible Galaxy](https://galaxy.ansible.com/joe-speedboat.virt_kvm)
```
ansible-galaxy install joe-speedboat.virt_kvm
```

Install from [Github](https://github.com/joe-speedboat/joe-speedboat.virt_kvm)
```
git clone https://github.com/joe-speedboat/joe-speedboat.virt_kvm.git joe-speedboat.virt_kvm
```

## Usage
Example playbooks for this role are located in `test` folder:
* `tests/test.yml`

## License
https://opensource.org/licenses/LGPL-3.0
Copyright (c) Chris Ruettimann <chris@bitbull.ch>



```
