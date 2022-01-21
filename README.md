Role Name
=========

Ansible role for installing [InBucket](https://github.com/inbucket/inbucket)


Role Variables
--------------

The package works without anything needing changing, however you can check the [Defaults file](https://github.com/carandclassic/inbucket-ansible/blob/main/defaults/main.yml) for any of the variables you want to override.
You can find information on the full config here: https://www.inbucket.org/configurator/


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: carandclassic.inbucket }

Laravel
-------

If you're using with Laravel you'll want the following in your .env, replacing appropriately if you've overriden the default values
```
MAIL_DRIVER=smtp
MAIL_HOST=localhost
MAIL_PORT=2500
```

License
-------

MIT

Author Information
------------------
- [Daniel Simkus](https://github.com/danielsimkus)
- [Car&Classic](https://github.com/carandclassic)
