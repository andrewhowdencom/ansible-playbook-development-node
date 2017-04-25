# Ansible Development Machine

Some work to create my dev machine because I'm lazy. I did this once before, but it was hard, and I haven't used it
as much as I should.

## Requirements

This playbook makes the presumption that the underlying machine is Debian Stretch.

The roles (where it seems reasonable) are developed separately and vendored into this repo using submodules; those
modules are re-usable, this playbook is not.

## Usage

The following command will execute the playbook:

```
$ ansible-playbook -i inventory development-node.yml
```

## Thanks

## Me

- Contact: hello@andrewhowden.com
- Web:     https://www.andrewhowden.com/
