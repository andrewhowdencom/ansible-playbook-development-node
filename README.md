# Ansible Display

This is the Display implementation of Ansible. It runs a series of tasks designed to set the expected state in Ansible.

i## Customization

If there are tasks that are specific to this property, create roles for them. If the tasks can be used, create them in
another repository, and add that repository as a submodule to this one

## Initial Setup

There are a few small tasks that must be performed separately to the Ansible provisioning. These include:

1. Resize the root partition
2. Enable SSH

Both of these tasks can be enabled with the `raspi-config` tool.

## Execution Instruction

The following command will execute the playbook:

```
$ ansible-playbook -i inventory display.yml
```

Authentication is handled out of band; it assumes that the user will have the appropriate `${HOME}/.ssh/config` file
set up. Such a file will look something like the following:

```
Host dp*
    User pi
    IdentityFile path/to/the/private/key.pem
```

## Thanks

- Vital K (https://github.com/vitalk) for instruction on how to disable SSH

## Me

- Contact: hello@andrewhowden.com
- Web:     https://www.andrewhowden.com/
