postgresql-rep-wal
=========

Роль для ansible. Настраивает репликацию PostgreSQL на основе трансляции журнала (WAL).

Requirements
----------

Для платформы: CentOS

Checked for Postgresql version: 10.6, 11.1

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

License
-------

MIT

Author Information
------------------

Alexey Matveev (c)
