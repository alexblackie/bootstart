# Bootstart

This is a repository of Ansible playbooks and roles that configure my laptops
and workstations.

## Prerequisites

These playbooks support only the latest releases of:

  - Fedora Workstation
  - Ubuntu (LTS)
  - macOS
    - (Homebrew must be installed first.)

Most tasks will probably work on RHEL/CentOS, but that is not tested nor
officially supported.

## Running

Run these playbooks as an unprivileged user (with `sudo` access). Pass
`--ask-become-pass` to have Ansible prompt for `sudo` authentication before
running.

```
$ ansible-playbook --ask-become-pass workstation.yml
```

There are two playbooks available:

  - `workstation.yml` for desktop/laptop workstations (GUI tools included);
  - `headless.yml` for headless Linux installs (CLI tools only).

## License

See [LICENSE](./LICENSE).
