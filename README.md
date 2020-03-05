postgresql-rep-wal
=========

Роль для ansible. Настраивает репликацию PostgreSQL на основе трансляции журнала (WAL).

Для платформы: CentOS

Role Variables
--------------

| Name              | Default Value       | Description          |
|-------------------|---------------------|----------------------|
| `pgsqlrep_role` | `skip` | `master` or `replica`, which determines which tasks run on the host. |
| `postgresql_conf_dir` |  |  |

Dependencies
------------

Каталог для архивирования должен существовать (pgsqlrep_archiv_path).

Пакеты: python-psycopg2

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

MIT

Author Information
------------------

Alexey Matveev (c)
