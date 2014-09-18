# Open-Transactions build machine

These Vagrant/Ansible scripts allow you to build the deb packages for the
[Open-Transactions project](https://github.com/Open-Transactions/opentxs).

## Prerequisites
- Virtualbox
- Vagrant
- Ansible

## Usage

```shell
$ vagrant up
$ scp -P 2222 ~/.ssh/id_rsa.pub vagrant@127.0.0.1:./.ssh/authorized_keys
$ ansible-playbook -i hosts buildbox.yml
```

Then just log in and run cmake in the `build` directory with whatever flags are desired.
