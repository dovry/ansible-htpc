dovry.htpc-programs
=========

Install required software for HTPC functionality

Requirements
------------

none

Role Variables
--------------

vars/main.yml

```yaml
# users to be added to the group 'docker'
docker_users:
```

Dependencies
------------

dovry.htpc-bootstrap

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables
passed in as parameters) is always nice for users too:

```yaml
    - hosts: target
      roles:
         - { role: dovry.htpc-programs, docker_users: myuser }
```

License
-------

MIT
