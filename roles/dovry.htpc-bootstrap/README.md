dovry.htpc-bootstrap
=========

Prepare the target host to become an HTPC

Requirements
------------

none

Role Variables
--------------

vars/main.yml

```yaml
# folders to create
folders:

# mounted / present
disk_state:

# ls /dev/disk/by-id
disk_id:

# mount path
disk_mnt:

# filesystem type, ex. ext4, xfs, zfs, etc-
disk_fstype:

# fstab mount options
disk_opts:
```

Dependencies
------------

none

Example Playbook
----------------

```yaml
- hosts: target
  roles:
     - { role: dovry.htpc-bootstrap }
```

License
-------

MIT
