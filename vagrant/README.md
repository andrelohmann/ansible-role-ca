# Test your role with vagrant

Test your role with vagrant

## Prerequisites

* Virtualbox is installed
* Vagrant is installed
* vagrant up will install vagrant-hostmanager module

## Test process

```
cd vagrant
vagrant up
```

The vagrant role will be applied automatically during the vagrant up process.

### Test with molecule from inside vagrant

```
vagrant ssh
cd /etc/ansible/roles/ansible-role-ca
molecule test
```

### Test cases

SSH into the vm

```
vagrant ssh
```

and inspect the certificates and key being created in /opt/ca.
