Anyenv
======
Install [anyenv](https://github.com/anyenv/anyenv).

Anyenv is installed and configured (only bash is currently supported) in the home directory of the user used by ansible. Use `become` and `become_user` to changed the target user (see example below).

Requirements
------------
See `meta/main.yml`.

Role Variables
--------------
See `defaults/main.yml`.

Dependencies
------------
Depends on git being available in the target host.

Example Playbook
----------------
```
- name: Install anyenv
  hosts: all
  roles:
    - role: anyenv
      become: yes
      become_user: vagrant
```

TODO
----
- Install plugins
- Install **envs

License
-------
Released under the [MIT license](https://opensource.org/licenses/MIT).

Author Information
------------------
Luis Gracia while at [The Rockefeller University](https://www.rockefeller.edu):
- lgracia [at] rockefeller.edu
- GitHub at [luisico](https://github.com/luisico)
