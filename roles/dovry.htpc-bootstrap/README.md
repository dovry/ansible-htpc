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
# list of folders to create
folders:

# List of drives to mount via /etc/fstab
# ls /dev/disk/by-id
disk_id:

# List of mount paths, use in conjunction with disk_id
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
