mysql [![Build Status](https://travis-ci.org/xcezx/ansible-mysql.svg)](https://travis-ci.org/xcezx/ansible-mysql)
=========

install and configuration mysql

Role Variables
--------------

- `mysql_group`
- `mysql_user`
- `mysql_build_checkout_dest`
- `mysql_build_version`
- `mysql_version`
- `mysql_plugin`
- `mysql_basedir`
- `mysql_datadir`
- `mysql_port`
- `mysql_rc_script`
- `mysql_root_password`
- `mysql_config`
- `mysql_append_config`

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: xcezx.mysql }

License
-------

BSD
