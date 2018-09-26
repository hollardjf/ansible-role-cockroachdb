ansible-cockroachdb
===================

This role aims at deploying cockroachdb, standalone only yet.

Requirements
------------

- Ansible >= 2.5
- Debian 9

Role Variables
--------------

All variables which can be overridden are stored in [defaults/main.yml](defaults/main.yml) file as well as in table below.

| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
| `cockroachdb_version` | 2.0.5 | version
| `cockroachdb_archive_location` | https://binaries.cockroachdb.com/cockroach-v2.0.5.linux-amd64.tgz | archive location
| `cockroachdb_dir_app` | /opt/apps/cockroachdb/ | app directory
| `cockroachdb_dir_log` | /var/log/cockroachdb/ | logs dir
| `cockroachdb_dir_data` | /var/lib/cockroachdb/ | data dir
| `cockroachdb_user` | cockroachdb | user who will launch the db
| `cockroachdb_group` | cockroachdb | user's group who will launch the db

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - role: ansible-role-cockroachdb

License
-------

This project is licensed under MIT License. See [LICENSE](/LICENSE) for more details.



