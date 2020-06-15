dovry.htpc-bootstrap
=========

Prepare the target host to become an HTPC

Requirements
------------

none

Role Variables
--------------

defaults/main.yml

```yaml
folders:
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
