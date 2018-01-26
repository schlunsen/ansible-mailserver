# ansible-postfix-dkim
Ansible role for opendkim with postfix configuration on Ubuntu & CentOS.

Tested against both Ubuntu 16.04 & CentOS 7.

### Example playbook
```yaml
---
- hosts: myserver
  user: root
  sudo: False
  roles:
    - role: BobbleSolutions.postfix-dkim
      dkim_selector: mail
      dkim_domains:
       - domain1.tld
       - domain2.tld
```

### Author Information

Latest revision by Christopher Davidson (chris@bobblesolutions.co.uk).

Forked from both https://github.com/gorazio/ansible-dkim & https://github.com/sunfoxcz/ansible-dkim.
