## Ansible and vagrant experiments

Personal experiments in ansible and vagrant.

## Prerequisites

- Install [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)
- Install [Vagrant](https://www.vagrantup.com/docs/installation)
- Install [Virtualbox](https://www.virtualbox.org/wiki/Downloads)

### WSL (Windows Subsystem for Linux)

I'm running my experiments on WSL v2. For that there's some extra points to watch out for:

- Fix [connection refused error on WSL v2](https://github.com/Karandash8/virtualbox_WSL2);
- Run `source setup-vagrant-wsl.sh`;

## How to run

```shell
cd chapter2
vagrant up
```

## Other notes

Test if ansible can reach a host with `ping`:
```shell
ansible -i inventory example -m ping -u filipe --ask-pass
```

### Other docs

- https://www.vagrantup.com/docs/other/wsl
- https://www.youtube.com/watch?v=goclfp6a2IQ&list=PL2_OBreMn7FqZkvMYt6ATmgC0KAGGJNAN
