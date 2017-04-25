# Ansible Development Machine

Some work to create my dev machine because I'm lazy. I did this once before, but it was hard, and I haven't used it
as much as I should.

## Requirements

This playbook makes the presumption that the underlying machine is Debian Stretch.

The roles (where it seems reasonable) are developed separately and vendored into this repo using submodules; those
modules are re-usable, this playbook is not.

## Release Tracks

There are three release tracks:

### Development

Things that I am testing out. Likely this will be everything, unless this development stack gets picked up by a
colleague.

### Canary

Things that are expected to be stable, but are only being rolled out on an elected basis such that more experienced
users can debug them.

### Stable

Things that should be working all day, every day.

## Usage

The following command will execute the playbook:

## Installation

It's expected this playbook will be "installed" by cloning it somewhere, and running it 1.x. After that, it will run by
itself every so often to ensure the state is as it expects, and propagate upgrades as they're required.

```
$ git clone https://github.com/andrewhowdencom/ansible-playbook-development-node.git /opt/ansible/
$ cd /opt/ansible/
$ ansible-playbook --inventory=inventory --extra-vars="release_track=stable" development-node.yml
```

## Additional Variables

You can store additional variables in the system wide path where they willl be discovered:

```
/etc/ansible/host_vars/localhost
```

For more information, see http://docs.ansible.com/ansible/playbooks_variables.html#variable-examples

## Thanks

## Me

- Contact: hello@andrewhowden.com
- Web:     https://www.andrewhowden.com/
