# Ansible Role: i3wm

An Ansible role that installs and configures [i3wm](https://i3wm.org/). This
install is likely to be opinionated towards how I use it, but I endevour to -
evenually - make essentiall everything configurable with the right set of
variables.

At several points, it may draw inspiration from similar projects, such as
[chaos-bodensee/role-i3wm](https://github.com/chaos-bodensee/role-i3wm) or
[hypebeast/ansible-i3](https://github.com/hypebeast/ansible-i3). As much as
anything, I'm using this as a learning experience for myself.

No guarantees are made as to any kind of suitablilty or reliability of this
playbook!

## Requirements

There are no requirements on the managed machine, though note that this is
designed to be run locally. As such, you may need the ansible tools installed
on the machine in question.

## Role Variables

TODO: Add these

```yaml
i3wm_execs:
  - command
  - othercommand
  - --no-startup-id command
i3wm_always_execs:
  - command
  - othercommand
  - --no-startup-id command
```
See [the i3wm doc](https://i3wm.org/docs/userguide.html#_automatically_starting_applications_on_i3_startup) for how these work. Commands should be specified in their relevant list.

## Dependencies

None.
