# Ansible Role: tuned

An Ansible role that deploys and configures [tuned][01] on Linux boxes.

## 🚀 Motivation

From tuned's [site][01]:

*TuneD is a system tuning service for Linux.* It *tunes system settings according to a selected profile* and *supports various types of configuration like `sysctl`, `sysfs`, or kernel boot command line parameters, which are integrated in a plug-in architecture*.

This role deploys and configures [tuned][01] on Linux boxes.

## 📑 Role Variables

Check [defaults/main.yml][02].

## 🧰 Dependencies

None.

## ⚡ Quick start

An example of how integrate this role to an Ansible playbook can be found here:

```yml
---
- name: Deploy tuned
  hosts: all
  become: true
  gather_facts: true
  roles:
    - fernandobohrer.tuned
```

## ⚙️ Compatibility

This role was tested on and is confirmed to work with the following Linux distributions:

- `Debian 13`
- `Ubuntu 24.04`

Details can be found in the [Molecule][03] scenarios available in the `molecule` folder.

## ⚠️ Warning

This Ansible role was tested on the above mentioned Linux distributions considering their default configuration. Your environment might have a different configuration or requirements which might conflict with the options that this role uses.

With the above in mind, it is **imperative** that you familiarize yourself with what this role does and test it on non-production machines **before** applying it to machines in a production environment.

## 📝 License

This project is licensed under the terms of the [MIT license][04].

[01]: https://tuned-project.org/
[02]: defaults/main.yml
[03]: https://github.com/fernandobohrer/ansible-molecule-scenarios
[04]: /LICENSE
