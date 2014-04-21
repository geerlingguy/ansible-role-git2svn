# Ansible Role: KDE's Svn2Git

Installs KDE's Svn2Git, a tool for quickly and easily converting SVN repositories to Git repositories, on any RHEL/CentOS Linux system.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `vars/main.yml`):

    workspace: /root

Where certain files will be downloaded and built for git2svn installation.

    svn2git_install_path: /usr/local/share

The location where svn2git will be installed.

    svn2git_qmake_bin_path: /usr/lib64/qt4/bin/qmake

The path to the `qmake` binary executable. This could differ slightly based on where QT4 is installed on your system.

## Dependencies

  - geerlingguy.svn
  - geerlingguy.git

## Example Playbook

    - hosts: servers
      roles:
        - { role: geerlingguy.git }

## License

MIT / BSD

## Author Information

This role was created in 2014 by [Jeff Geerling](http://jeffgeerling.com/), author of [Ansible for DevOps](http://ansiblefordevops.com/).
