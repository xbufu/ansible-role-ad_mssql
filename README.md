Ansible Role: MSSQL Server
=========

An Ansible role to set up an MSSQL instance with SSMS.

Requirements
------------

None.

Role Variables
--------------

```yml
sql_iso_path: '\\pdc01\Resources\SQLServer2019-x64-ENU.iso'
ssms_setup_path: '\\pdc01\Resources\SSMS-Setup-ENU.exe'
sql_version: '2019'
sql_config_path: 'C:\ConfigurationFile.ini'
sql_license_key: ''
sql_instance_name: sql01
sql_service_user: 'ad01\administrator'
sql_service_password: 'Password!'
sql_admin_accounts: 'ad01\administrator'
```

Dependencies
------------

None.

Example Playbook
----------------

```yml
- hosts: sql01
  roles:
    - role: xbufu.ad_mssql
      vars:
        sql_iso_path: '\\pdc01\Resources\SQLServer2019-x64-ENU.iso'
        ssms_setup_path: '\\pdc01\Resources\SSMS-Setup-ENU.exe'
        sql_version: '2019'
        sql_config_path: 'C:\ConfigurationFile.ini'
        sql_license_key: ''
        sql_instance_name: sql01
        sql_service_user: 'ad01\administrator'
        sql_service_password: 'Password!'
        sql_admin_accounts: 'ad01\administrator'
```

License
-------

MIT / BSD

Author Information
------------------

Created by xbufu.
