Locale Configuration
====================

Generates and sets the specified system locale files for target hosts.

Requirements
------------

The only requirements for this role are a Debian host with the `locale-gen` and `dpkg-reconfigure` commands.

Role Variables
--------------

This role contains a single variable:

```yaml
ansible-locales:
```


Example Playbook
----------------

_Default Locales (en\_US and en\_CA)_
```yaml
- hosts: servers
  roles:
    - { role: amaabca.ansible-locale }
```

_With Custom Locales_
```yaml
- hosts: servers
  roles:
    - { role: amaabca.ansible-locale, ansible_locales: ['en_HK'] }
```

License
-------

MIT

Author Information
------------------

Built by the web team at [AMA](https://ama.ab.ca) - https://github.com/amaabca.
