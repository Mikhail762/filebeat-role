Filebeat role
=========

Роль для установки filebeat на хостах с ОС: Debian, Ubuntu, CentOS, RHEL.

Requirements
------------

Поддерживаются только ОС семейств debian и RHEL.

Role Variables
--------------

| Variable name | Default | Description |
|-----------------------|----------|-------------------------|
| filebeat_version | "7.14.0" | Параметр, который определяет какой версии filebeat будет установлен |
| filebeat_rpm_url | "https://artifacts.elastic.co/downloads/beats/filebeat/filebeat-{{ elk_stack_version }}-x86_64.rpm" | Ссылка на rpm-дистрибутив filebeat|
| filebeat_deb_url | "https://artifacts.elastic.co/downloads/beats/filebeat/filebeat-{{ elk_stack_version }}-x86_64.deb" | Ссылка на deb-дистрибутив filebeat|

Example Playbook
----------------

    - hosts: all
      roles:
         - { role: mnt-homeworks-ansible }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
