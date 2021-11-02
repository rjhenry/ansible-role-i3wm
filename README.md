# Ansible Role: i3wm

[![CI](https://img.shields.io/gitlab/pipeline/rjh/ansible-role-i3wm/main?gitlab_url=https%3A%2F%2Fgitlab.rickhenry.uk)](https://gitlab.rickhenry.uk/rjh/ansible-role-i3wm/-/commits/main)
[![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/rjhenry/ansible-role-i3wm?sort=semver)]()
[![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/rjhenry/ansible-role-i3wm)]()

[![Ansible Role](https://img.shields.io/ansible/role/56008)](https://galaxy.ansible.com/rjhenry/i3wm) 
[![Ansible Role Downloads](https://img.shields.io/ansible/role/d/56008)](https://galaxy.ansible.com/rjhenry/i3wm) 
[![Ansible Quality Score](https://img.shields.io/ansible/quality/56008)](https://galaxy.ansible.com/rjhenry/i3wm) 

There are two copies of this repository! There is my
[GitLab](https://gitlab.rickhenry.uk/rjh/ansible-role-i3wm), and a copy on
[GitHub](https://github.com/rjhenry/ansible-role-i3wm). The GitLab copy is the
primary!

An Ansible role that installs and configures [i3wm](https://i3wm.org/). This
install is likely to be opinionated towards how I use it, but I endevour to -
evenually - make essentially everything configurable with the right set of
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

i3wm_other_binds:
  - keybind: "$mod+Shift+d"
    action: rofi-pass
```
See
[the i3wm doc](https://i3wm.org/docs/userguide.html#_automatically_starting_applications_on_i3_startup)
for how these work. Commands should be specified in their relevant list.

## Dependencies

None.

## Contributing
If you feel the need to contribute to this role, please create
[issues](https://gitlab.rickhenry.uk/rjh/ansible-role-i3wm/-/issues) on the
project. If you have patches you'd like to submit, create a PR on GitHub, from
where I'll pull those changes to GitLab.
