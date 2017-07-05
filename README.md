Gentoo Upgrader via Historical Portage Snapshots
================================================

Ansible playbook to upgrade old Gentoo systems using historical portage
snapshots.

[Portage archives](https://dev.gentoo.org/~swift/snapshots/)
[Documentation Reference](https://wiki.gentoo.org/wiki/Upgrading_Gentoo#Upgrading_from_older_systems)


Quick start
-----------

1. Run the playbook

> ansible-playbook upgrade.yml


Usage
-----

1. Populate a ansible hosts file, pointing towards the system(s) that require
   upgrading.

2. Edit upgrade.yml, modifying the parameterised roles with the dates of the
   snapshots that are required.

3. Run the playbook, passing the hosts line that corresponds to the upgrading
   systems

> ansible-playbook -i hostsfile upgrade.yml -e hosts=myhost
