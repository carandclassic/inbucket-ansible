# inbucket-ansible
Ansible role for installing InBucket https://github.com/inbucket/inbucket

# How to use

The package works without anything needing changing, however you can check `defaults/main.yml` for any of the variables you want to override.
You can find information on the full config here: https://www.inbucket.org/configurator/

Add the `carandclassic.inbucket-ansible` role in your playbook
```
roles:
    - { role: carandclassic.inbucket-ansible, tags: ["inbucket"] }
```

# Laravel
If you're using with Laravel you'll want the following in your .env, replacing appropriately if you've overriden the default values
```
MAIL_DRIVER=smtp
MAIL_HOST=localhost
MAIL_PORT=2500
```

# Accessing the webpanel
By default the webpanel should be accessible on port `9000`:
`http://{yourVMIpAddress}:9000`

If you want to use localhost, you will have to setup portforwarding in vagrant 👍
