letsencrypt_sh
=================

Ansible Role for Let's Encrypt usign letsencrypt.sh

Requirements
------------


Role Variables
--------------

```
letsencrypt_domains:
  - email: "hostmaster@exmaple.com"
    domains: ["example.com", "www.example.com"]
  - email: "git@exmaple.com"
    domains: ["git.example.com", "gitlab.example.com"]

#current supported hook 
letsencrypt_sh_hook_name: 'dnspod'
letsencrypt_sh_hook_dnspod_login_token: "111:some-dnspod token"
letsencrypt_sh_hook_dnspod_dns_servers: "f1g1ns1.dnspod.net f1g1ns2.dnspod.net"
```


Dependencies
------------


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: ftao.letsencrypt_sh}

License
-------

MIT

Author Information
------------------

https://github.com/ftao/ansible-role-letsencrypt-sh
